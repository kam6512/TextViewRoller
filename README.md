# TextViewRoller

this source code Based by Hsd

[link](http://www.androidpub.com/2472793)


```java
public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        final RollingItem item1 = (RollingItem) findViewById(R.id.MainRollingItem1);
        final RollingItem item2 = (RollingItem) findViewById(R.id.MainRollingItem2);
        final RollingItem item3 = (RollingItem) findViewById(R.id.MainRollingItem3);
        final RollingItem item4 = (RollingItem) findViewById(R.id.MainRollingItem4);
        final RollingItem item5 = (RollingItem) findViewById(R.id.MainRollingItem5);

        findViewById(R.id.MainBtnRoll).setOnClickListener(new View.OnClickListener() {

            @Override
            public void onClick(View v) {
                item1.startRolling(2,11);
                //startRolling(value, rollCount)
                item2.startRolling(3,22);
                item3.startRolling(4,33);
                item4.startRolling(1,44);
                item5.startRolling(0,55);
            }
        });
    }
}
```
