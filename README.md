# react-native-mic-stream

React Native module used for two-way audio

## Install

```
$ npm i git://github.com/oscarmuya/react-native-mic-stream.git
$ react-native link react-native-mic-stream
```

## Usage

```javascript
import MicStream from 'react-native-mic-stream';

const listener = MicStream.addListener(data => console.log(data));
MicStream.init({
  bufferSize: 4096,
  sampleRate: 44100,
  bitsPerChannel: 16,
  channelsPerFrame: 1,
});
MicStream.start();
...
MicStream.stop();
listener.remove();
```
