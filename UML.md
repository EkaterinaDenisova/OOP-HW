# UML-диаграмма

```text
@startuml
class Time 
{
  - int days;
  - int hours;
  - int minutes;
  - int seconds;


   + Time();
   + Time(int d, int h, int m, int s);                            
   + void set_time_in_seconds (int t);
   + void set_time (int d, int h, int m, int s);
   + void set_seconds(int s);
   + void set_minutes(int m);
   + void set_hours(int h);
   + void set_days(int d);

   + int get_seconds() const;
   + int get_minutes() const;
   + int get_hours() const;
   + int get_days() const;  

   + void add_time (int d, int h, int m, int s);
   + void subtract_time (int d, int h, int m, int s);

   + static int convert_to_seconds (int d, int h, int m, int s);
   + static float convert_to_minutes (int d, int h, int m, int s);
   + static float convert_to_hours (int d, int h, int m, int s);
   + static float convert_to_days (int d, int h, int m, int s);

   + std::string to_string();   
}
@enduml
```

![](UML_diagram.png)
