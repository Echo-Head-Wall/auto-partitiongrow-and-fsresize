# auto-partitiongrow-and-fsresize
have you ever locked your self out a system can resize the virtual hardrive but cant do anything in your machine while this will fix that and just make it so you dont have to worry about manually resizing



cp ./resize-partition.service /etc/systemd/system/resize-partition.service
cp ./resize-partition.timer /etc/systemd/system/resize-partition.timer
sudo systemctl daemon-reload
sudo systemctl start resize-partition.timer
sudo systemctl enable resize-partition.timer
