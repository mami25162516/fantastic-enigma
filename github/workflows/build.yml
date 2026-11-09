package com.example.jarvis;

import android.app.*;
import android.os.*;
import android.graphics.Color;
import android.view.Gravity;
import android.widget.*;

public class MainActivity extends Activity {

    LinearLayout layout;
    EditText mesaj;
    TextView sohbet;

    @Override
    public void onCreate(Bundle b) {
        super.onCreate(b);

        layout = new LinearLayout(this);
        layout.setOrientation(1);
        layout.setPadding(25,25,25,25);
        layout.setBackgroundColor(Color.rgb(5,12,28));

        TextView baslik = new TextView(this);
        baslik.setText("J.A.R.V.I.S.");
        baslik.setTextSize(30);
        baslik.setTextColor(Color.CYAN);
        baslik.setGravity(Gravity.CENTER);
        layout.addView(baslik);

        sohbet = new TextView(this);
        sohbet.setText("JARVIS hazır. Size nasıl yardımcı olabilirim?");
        sohbet.setTextColor(Color.WHITE);
        sohbet.setTextSize(18);
        layout.addView(sohbet);

        mesaj = new EditText(this);
        mesaj.setHint("JARVIS'e yaz...");
        layout.addView(mesaj);

        Button gonder = new Button(this);
        gonder.setText("GÖNDER");
        layout.addView(gonder);

        gonder.setOnClickListener(v -> {
            String m = mesaj.getText().toString();
            sohbet.append("\\n\\nSen: " + m);
            sohbet.append("\\nJARVIS: Mesajını aldım.");
            mesaj.setText("");
        });

        setContentView(layout);
    }
}
