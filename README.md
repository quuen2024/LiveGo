# LiveGo
<!DOCTYPE html>
<html lang="en">
    <head>
{
  "name": "nsplayer",
  "version": "0.7.0",
  "description": "NSPlayer, a player which supports quality list of dash and hls",
  "keywords": [
    "nsplayer",
    "dash.js",
    "hls.js"
  ],
  "license": "MIT",
  "author": "tangye <tangye@xinpainchang.com> ([https://github.com/tangye1234](https://github.com/quuen2024/LiveGo))",
  "main": "dist/cjs/index.js",
  "module": "dist/esm/index.js",
  "types": "dist/types/index.d.ts",
  "files": [
    "dist"
  ],
  "repository": "github:xinpianchang/nsplayer",
  "publishConfig": {
    "registry": "https://registry.npmjs.org"
  },
  "scripts": {
    "prebuild": "npm run test && npm run clean",
    "build": "npm run build:types && npm run build:js",
    "build:js": "rollup -c",
    "build:types": "tsc --emitDeclarationOnly",
    "clean": "rimraf dist",
    "lint": "eslint src/**/* --fix",
    "pretty": "prettier src/**/* --write",
    "prerelease": "npm run build",
    "release": "npx standard-version",
    "postrelease": "git push --follow-tags",
    "start": "NODE_ENV=development rollup -c -w --watch.exclude rollup.devserver.js",
    "pretest": "npm run lint",
    "test": "jest",
    "test:cov": "npm run test -- --coverage",
    "test:watch": "npm run test -- --watch --notify",
    "types:check": "tsc --noEmit",
    "types:watch": "npm run types:check -- --watch"
  },
  "husky": {
    "hooks": {
      "pre-commit": "lint-staged",
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
  },
  "commitlint": {
    "extends": [
      "@commitlint/config-conventional"
    ]
  },
  "lint-staged": {
    "*.{js,jsx,ts,tsx}": [
      "eslint --fix"
    ],
    "*.{json,md,yml}": [
      "prettier --write"
    ]
  },
  "devDependencies": {
    "@babel/cli": "^7.12.10",
    "@babel/core": "^7.12.10",
    "@babel/plugin-proposal-class-properties": "^7.12.1",
    "@babel/plugin-proposal-optional-chaining": "^7.12.7",
    "@babel/plugin-transform-runtime": "^7.12.10",
    "@babel/plugin-transform-typescript": "^7.12.1",
    "@babel/preset-env": "^7.12.11",
    "@babel/preset-typescript": "^7.12.7",
    "@commitlint/cli": "^11.0.0",
    "@commitlint/config-conventional": "^11.0.0",
    "@newstudios/common": "^0.2.2",
    "@rollup/plugin-babel": "^5.3.0",
    "@rollup/plugin-commonjs": "^21.0.1",
    "@rollup/plugin-json": "^4.1.0",
    "@rollup/plugin-node-resolve": "^13.1.1",
    "@rollup/plugin-replace": "^3.0.0",
    "@types/hls.js": "^1.0.0",
    "@types/jest": "^26.0.20",
    "@types/rollup-plugin-node-builtins": "^2.1.2",
    "@typescript-eslint/eslint-plugin": "^5.15.0",
    "@typescript-eslint/parser": "^5.15.0",
    "eslint": "^8.5.0",
    "eslint-config-prettier": "^8.3.0",
    "eslint-plugin-jest": "^25.3.0",
    "eslint-plugin-prettier": "^4.0.0",
    "husky": "^4.3.8",
    "jest": "^26.6.3",
    "lint-staged": "^10.5.3",
    "prettier": "^2.5.1",
    "rimraf": "^3.0.2",
    "rollup": "^2.70.1",
    "rollup-plugin-node-builtins": "^2.1.2",
    "rollup-plugin-serve": "^1.1.0",
    "rollup-plugin-terser": "^7.0.2",
    "ts-node": "^9.1.1",
    "typescript": "^4.6.2",
    "vconsole": "^3.13.0"
  },
  "dependencies": {
    "@babel/runtime": "^7.16.5",
    "dashjs": "^4.6.0",
    "delegates": "^1.0.0",
    "hls.js": "^1.3.5",
    "shaka-player": "^4.3.5"
  },
  "npmName": "nsplayer",
  "peerDependencies": {
    "@newstudios/common": "^0.2.2"
  }
}

12-29 14:56:19.769  i: [ExoPlayer][EventLogger] videoDisabled [eventTime=881.61, mediaPos=878.85, window=0, period=0]
12-29 14:56:19.782  i: [ExoPlayer][EventLogger] audioDisabled [eventTime=881.62, mediaPos=878.85, window=0, period=0]
12-29 14:56:19.810  e: [ExoPlayer][EventLogger] playerFailed [eventTime=881.64, mediaPos=878.85, window=0, period=0, errorCode=ERROR_CODE_DECODING_FAILED
  com.google.android.exoplayer2.r: MediaCodecVideoRenderer error, index=1, format=Format(0, null, null, video/dolby-vision, dvhe.07.06, -1, null, [3840, 2160, 23.976025], [-1, -1]), format_supported=NO_EXCEEDS_CAPABILITIES
      at com.google.android.exoplayer2.x1.handleMessage(SourceFile:363)
      at android.os.Handler.dispatchMessage(Handler.java:102)
      at android.os.Looper.loop(Looper.java:223)
      at android.os.HandlerThread.run(HandlerThread.java:67)
  Caused by: com.google.android.exoplayer2.video.h: Decoder failed: OMX.dolby.vision.dvhe.stn.decoder
      at com.google.android.exoplayer2.video.i.m(Unknown Source:4)
      at y3.p.render(SourceFile:154)
      at com.google.android.exoplayer2.x1.p(SourceFile:92)
      at com.google.android.exoplayer2.x1.handleMessage(SourceFile:221)
      ... 3 more
  Caused by: java.lang.IllegalStateException
      at android.media.MediaCodec.native_dequeueOutputBuffer(Native Method)
      at android.media.MediaCodec.dequeueOutputBuffer(MediaCodec.java:3452)
      at y3.y.k(SourceFile:5)
      at y3.p.drainOutputBuffer(SourceFile:45)
      at y3.p.render(SourceFile:72)
      ... 5 more
]
12-29 14:56:19.811  e: [Player][ExoPlayer] Playback error detected
12-29 14:56:19.819  e: An exception occurred: com.google.android.exoplayer2.r: MediaCodecVideoRenderer error, index=1, format=Format(0, null, null, video/dolby-vision, dvhe.07.06, -1, null, [3840, 2160, 23.976025], [-1, -1]), format_supported=NO_EXCEEDS_CAPABILITIES
12-29 14:56:19.821  i: [Player][Timeline] Handling player error
12-29 14:56:19.822  e: Stacktrace: com.google.android.exoplayer2.r: MediaCodecVideoRenderer error, index=1, format=Format(0, null, null, video/dolby-vision, dvhe.07.06, -1, null, [3840, 2160, 23.976025], [-1, -1]), format_supported=NO_EXCEEDS_CAPABILITIES
	at com.google.android.exoplayer2.x1.handleMessage(SourceFile:363)
	at android.os.Handler.dispatchMessage(Handler.java:102)
	at android.os.Looper.loop(Looper.java:223)
	at android.os.HandlerThread.run(HandlerThread.java:67)
Caused by: com.google.android.exoplayer2.video.h: Decoder failed: OMX.dolby.vision.dvhe.stn.decoder
	at com.google.android.exoplayer2.video.i.m(Unknown Source:4)
	at y3.p.render(SourceFile:154)
	at com.google.android.exoplayer2.x1.p(SourceFile:92)
	at com.google.android.exoplayer2.x1.handleMessage(SourceFile:221)
	... 3 more
Caused by: java.lang.IllegalStateException
	at android.media.MediaCodec.native_dequeueOutputBuffer(Native Method)
	at android.media.MediaCodec.dequeueOutputBuffer(MediaCodec.java:3452)
	at y3.y.k(SourceFile:5)
	at y3.p.drainOutputBuffer(SourceFile:45)
	at y3.p.render(SourceFile:72)
	... 5 more

#EXT-X-MEDIA-SEQUENCE:0
#EXT-X-ALLOW-CACHE:YES
#EXT-X-TARGETDURATION:11
#EXTINF:10.080000,
