# Passing-data-from-one-activity-to-another
XML Code for passing data from one activity to another
Main Activity XML Code:
<RelativeLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 tools:context=".MainActivity">
 <TextView
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:text="Registration"
 android:gravity="center"
 android:textSize="50dp"
 android:fontFamily="monospace"
 android:id="@+id/tv_main"/>
 <Button
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:text="Registration"
 android:layout_centerHorizontal="true"
 android:layout_marginTop="150dp"
 android:layout_below="@+id/tv_main"
 android:id="@+id/btn_registration"/>
</RelativeLayout>
Form Activity:
<LinearLayout 
xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 android:orientation="vertical"
 tools:context=".Form">
 <ScrollView
 android:layout_width="match_parent"
 android:layout_height="match_parent">
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 android:orientation="vertical"
 android:weightSum="7">
 <TextView
 android:id="@+id/tv"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:text="Registration"
 android:gravity="center"
 android:textSize="25sp" />
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:id="@+id/tv_name"
android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
android:text="Name" />
 <EditText
 android:id="@+id/edt_name"
android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:layout_weight="1"
android:hint="Name" />
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:weightSum="2">
 <TextView
 android:id="@+id/tv_FN"
android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:layout_weight="1"
 android:text="Father name" />
 <EditText
 android:id="@+id/edt_FN"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:layout_weight="1"
android:hint="Father Name" />
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:weightSum="2">
 <TextView
 android:id="@+id/tv_MN"
android:layout_width="match_parent"
android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Mother Name" />
 <EditText
 android:id="@+id/edt_MN"
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:layout_weight="1"
android:hint="Mother Name" />
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:weightSum="2">
 <TextView
 android:id="@+id/tv_age"
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Age" />
 <EditText
 android:id="@+id/edt_age"
android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:layout_weight="1"
android:hint="Age" />
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:weightSum="2">
 <TextView
 android:id="@+id/tv_gender"
android:layout_width="match_parent"
android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Gender" />
 <RadioGroup
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:layout_weight="1"
android:weightSum="3"
 android:id="@+id/rg">
 <RadioButton
 android:id="@+id/rb_male"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
 android:layout_weight="1"
 android:text="Male" />
 <RadioButton
 android:id="@+id/rb_female"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
 android:layout_weight="1"
android:text="Female" />
 <RadioButton
 android:id="@+id/rb_other"
android:layout_width="wrap_content"
 android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Others" />
 </RadioGroup>
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal"
 android:weightSum="2">
 <Button
 android:id="@+id/btn_submit"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Submit" />
 <Button
 android:id="@+id/btn_cancel"
 android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:layout_weight="1"
android:text="Cancel" />
 </LinearLayout>
 </LinearLayout>
 </ScrollView>
</LinearLayout>
CompleteForm:
<LinearLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 android:orientation="vertical"
 tools:context=".CompletedForm">
 <ScrollView
 android:layout_width="match_parent"
 android:layout_height="match_parent">
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 android:orientation="vertical"
 android:weightSum="5">
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:id="@+id/Tv_name"
android:text="Name : "
android:textSize="30sp"
android:layout_weight="1"/>
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_name_cf"
android:textSize="30sp"
android:layout_weight="1"/>
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_fn"
android:text="Father Name : "
android:textSize="30sp"
android:layout_weight="1"/>
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_fn_cf"
 android:textSize="30sp"
 android:layout_weight="1"/>
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_mn"
android:text="Mother Name:"
android:textSize="30sp"
android:layout_weight="1"/>
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_mn_cf"
android:textSize="30sp"
android:layout_weight="1"/>
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:id="@+id/Tv_age"
android:text="Age : "
android:textSize="30sp"
android:layout_weight="1"/>
 <TextView
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:id="@+id/Tv_age_cf"
android:textSize="30sp"
android:layout_weight="1"/>
 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:layout_weight="1"
 android:weightSum="2">
 <TextView
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
android:id="@+id/Tv_gender"
android:text="Gender : "
android:textSize="30sp"
 android:layout_weight="1"/>
 <TextView
 android:layout_width="match_parent"
android:layout_height="wrap_content"
android:id="@+id/Tv_gender_cf"
android:textSize="30sp"
 android:layout_weight="1"/>
 </LinearLayout>
 </LinearLayout>
 </ScrollView>
</LinearLayout>
JAVA Code for passing data from one activity to another
MainActivity:
public class MainActivity extends AppCompatActivity {
 Button button;
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
 button = findViewById(R.id.btn_registration);
 button.setOnClickListener(new View.OnClickListener() {
 @Override
 public void onClick(View v) {
 startActivity(new 
Intent(MainActivity.this,Form.class));
 }
 });
 }
}
Form.class: 
public class Form extends AppCompatActivity implements 
View.OnClickListener{
 protected TextView tv_name,tv_fn,tv_mn,tv_age,tv_gender;
 Button btn_submit,btn_cancel;
 EditText et_name,et_fn,et_mn,et_age;
 RadioGroup radioGroup;
 //RadioButton rb_m,rb_fm,rb_other;
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_form);
// tv_name=findViewById(R.id.tv_name);
// tv_fn=findViewById(R.id.tv_FN);
// tv_mn=findViewById(R.id.tv_MN);
// tv_age=findViewById(R.id.tv_age);
// tv_gender=findViewById(R.id.tv_gender);
 et_name = findViewById(R.id.edt_name);
 et_fn = findViewById(R.id.edt_FN);
 et_mn = findViewById(R.id.edt_MN);
 et_age = findViewById(R.id.edt_age);
 radioGroup = findViewById(R.id.rg);
 //radioGroup.setOnCheckedChangeListener(this);
// rb_m= findViewById(R.id.rb_male);
// rb_fm= findViewById(R.id.rb_female);
// rb_other= findViewById(R.id.rb_other);
 btn_submit= findViewById(R.id.btn_submit);
 btn_cancel= findViewById(R.id.btn_cancel);
 btn_submit.setOnClickListener(this);
 btn_cancel.setOnClickListener(this);
 }
 @Override
 public void onClick(View v) {
 if (v.getId() == R.id.btn_submit){
 String name = et_name.getText().toString();
 String F_name = et_fn.getText().toString();
 String M_name = et_mn.getText().toString();
 String age = et_age.getText().toString();
 int genderID = radioGroup.getCheckedRadioButtonId();
 Intent i = new 
Intent(Form.this,CompletedForm.class);
 i.putExtra("NAME",name);
 i.putExtra("F_NAME",F_name);
 i.putExtra("M_NAME",M_name);
 i.putExtra("AGE",age);
 switch (genderID){
 case R.id.rb_male:
 i.putExtra("gender","Male");
 break;
 case R.id.rb_female:
 i.putExtra("gender","Female");
 break;
 case R.id.rb_other:
 i.putExtra("gender","Other");
 break;
 }
 startActivity(i);
 }else if (v.getId() == R.id.btn_cancel){
 startActivity(new 
Intent(Form.this,MainActivity.class));
 
Toast.makeText(getApplicationContext(),"Registration",Toast.LENG
TH_LONG).show();
 }
 }
}
CompleteFrom: 
public class CompletedForm extends AppCompatActivity {
 TextView tv_name,tv_fn,tv_mn,tv_age,tv_gender;
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_completed_form);
 tv_name= findViewById(R.id.Tv_name_cf);
 tv_fn= findViewById(R.id.Tv_fn_cf);
 tv_mn= findViewById(R.id.Tv_mn_cf);
 tv_age= findViewById(R.id.Tv_age_cf);
 tv_gender= findViewById(R.id.Tv_gender_cf);
 tv_name.setText(getIntent().getStringExtra("NAME"));
 tv_fn.setText(getIntent().getStringExtra("F_NAME"));
 tv_mn.setText(getIntent().getStringExtra("M_NAME"));
 tv_age.setText(getIntent().getStringExtra("AGE"));
 tv_gender.setText(getIntent().getStringExtra("gender"));
 }
}
