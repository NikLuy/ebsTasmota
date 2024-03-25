# ebsTasmota
Diese version von Tasmota ist eine variante der Tasmota software, mit einstellungen für den Smartmeter L&G 360 
Die Installation und Einstelleungen sind relativ einfach. 

Die Firmware muss wegen der Grösse allenfalls per USB Kabel auf den Tasmota geladen werden. 
##Script
Anschliessend unter 
Tools
![image](https://github.com/NikLuy/ebsTasmota/assets/7451747/9fd86a51-58a3-4d80-9c52-2e82832a23ea)

Edit Script
![image](https://github.com/NikLuy/ebsTasmota/assets/7451747/856d40e3-f778-4f03-aeaf-6496f9e38ba2)

Den Inhalt von TasmotaScript einfügen. 
![image](https://github.com/NikLuy/ebsTasmota/assets/7451747/7e514ff7-416e-465b-9ebd-ba3c168a32c1)

###
Sollen die Werte an einen MQTT Server gesendet werden, kann die Updaterate anhand der letzten Zahl des Gewünschten Wertes in der Sektion >M angepasst werden.
0-15 sind die Anzahl Kommastellen des Wertes und werden anhand des TelePeriod parameter upgedatet. Hier liegt der Minimalwert bei 10s
16-31 sind die Anzahl Kommastellen + 16 und werden sofort bei Wertänderung an den Mqtt Server gesendet. Dies hat zur folge, dass beim Topic jeweils nur ein Wert ersichtlich ist, da alle nacheinander gesendet werden.

##GUI
Das GUI zeigt alle Werte, welche über den SmartMeter L&G ausgelesen werden können. 
Nur die Blindleistungen habe ich weggelassen. 
![image](https://github.com/NikLuy/ebsTasmota/assets/7451747/e2b9d342-4ddb-4041-a1db-78ddab48bee7)