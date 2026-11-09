# 선명하게 — AI 사진 확대

브라우저에서 사진을 2, 3, 4배로 확대하는 정적 웹 앱입니다. 사진은 브라우저에서 처리하며 서버로 업로드하지 않습니다. 첫 실행에는 모델과 ONNX Runtime을 다운로드합니다. 큰 사진은 느리거나 기기의 메모리가 부족할 수 있습니다.

## 사용법

GitHub Pages 사이트에 접속해 사진을 선택하고 배율을 정한 뒤 확대 버튼을 누르세요. 완료 후 PNG로 다운로드할 수 있습니다. 파일 용량 제한은 없지만 브라우저 메모리를 고려해 결과 이미지가 6400만 픽셀 또는 한 변 16384 픽셀을 넘으면 배율을 낮춰야 합니다. 기기에 따라 더 작은 사진에서도 메모리가 부족할 수 있습니다.

## 기술과 출처

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN): BSD 3-Clause
- [브라우저용 Real-ESRGAN ONNX 모델](https://huggingface.co/Saimon8420/realesr-general-x4v3-web): BSD 3-Clause
- [ONNX Runtime Web](https://github.com/microsoft/onnxruntime): MIT

모델과 실행 도구는 외부 서비스에서 내려받으며 해당 서비스 및 네트워크 상태에 영향을 받습니다. AI가 추정한 디테일은 원본과 다를 수 있습니다.
