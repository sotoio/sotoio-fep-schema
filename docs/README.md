# FEP Schema Repository

## 목적
방사성 폐기물 처분 안전성 평가를 위한 FEP(FEatures, Events, Processes) 데이터셋 구조를 표준화합니다.

## 구성
- schema/: JSON Schema 정의 (unified, core)
- examples/: 예시 데이터
- docs/: 문서
- validation/: 검증 가이드

## 검증 방법
```bash
pip install jsonschema
jsonschema -i examples/example_normal_evolution.json schema/fep-unified.schema.json
```

또는 Node.js 환경에서:
```bash
npm install -g ajv-cli
ajv validate -s schema/fep-unified.schema.json -d examples/example_normal_evolution.json
```

## 버전
- 1.0.0: 최초 공개
