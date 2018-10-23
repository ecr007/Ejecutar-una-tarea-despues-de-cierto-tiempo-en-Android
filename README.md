# Ejecutar una tarea despues de cierto tiempo en Android

```java
Thread thread = new Thread() {
    @Override
    public void run() {
        try {
            while(true) {
                sleep(1000);
                handler.post(this);
            }
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
};

thread.start();
```


```java
Thread thread = new Thread(){
    @Override
    public void run(){
        dialog.dismiss();
    }
};

thread.start();
```
