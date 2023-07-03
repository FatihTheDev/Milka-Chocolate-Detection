import cv2

trainingData = cv2.CascadeClassifier("milka.xml")

webcam = cv2.VideoCapture(0)

while 1:
    successful_frame_read, frame = webcam.read()

    grayscaled_recording = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    milka_detected = trainingData.detectMultiScale(grayscaled_recording, scaleFactor = 1.12, minNeighbors = 33)

    for (x, y, w, h) in milka_detected:
        cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 0), 3)
        cv2.putText(frame, 'Milka detected', (x, y+h+40), fontScale=3, fontFace=cv2.FONT_HERSHEY_PLAIN, color=(0,255,0))

    cv2.imshow('Milka chocolate detector', frame)
    key = cv2.waitKey(1)

    if(key == 81 or key == 113):
        break
        
webcam.release()
cv2.destroyAllWindowsimport cv2

trainingData = cv2.CascadeClassifier("milka.xml")

webcam = cv2.VideoCapture(0)

while 1:
  successful_frame_read, frame = webcam.read()

  grayscaled_recording = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

  milka_detected = trainingData.detectMultiScale(grayscaled_recording, scaleFactor = 1.12, minNeighbors = 33)

  for (x, y, w, h) in milka_detected:
    cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 0), 3)
    cv2.putText(frame, 'Milka detected', (x, y+h+40), fontScale=3, fontFace=cv2.FONT_HERSHEY_PLAIN, color=(0,255,0))

  cv2.imshow('Milka chocolate detector', frame)
    key = cv2.waitKey(1)

  if(key == 81 or key == 113):
    break
        
webcam.release()
cv2.destroyAllWindows
