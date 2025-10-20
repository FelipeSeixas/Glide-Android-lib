import android.app.Activity;
import android.content.Intent;
import android.os.Bundle;
import android.os.Handler;
import android.widget.ImageView;

import com.bumptech.glide.Glide;

public class Splash extends Activity {

    ImageView imgGlide;
    String img = "https://jangadashow.com.br/wp-content/uploads/2023/03/paisagem-praia-ponta-negra-morro-do-careca-natal.jpg";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_splash);

        imgGlide = findViewById(R.id.iv_splash);
        Glide.with(this)
                .load(img).into(imgGlide);

        new Handler().postDelayed(new Runnable() {
            @Override
            public void run() {
                startActivity(new Intent(getBaseContext(),DadosActivity.class));
                finish();
            }
        },3000);
    }
}
