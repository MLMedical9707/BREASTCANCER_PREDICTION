# 🏥 유방암 진단 데이터 분석 프로젝트

## 📌 개요
본 프로젝트는 **Breast Cancer Wisconsin (Diagnostic) 데이터셋**을 활용하여 **유방암 진단 모델을 개발**하고, **양성(Benign)과 악성(Malignant) 종양을 분류**하는 것을 목표로 합니다.  

- **데이터셋 출처:** [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)  
- **샘플 수:** 569개  
- **특성 수:** 30개 (세포 핵 특성)  
- **결측값 없음**  

## 🔎 데이터 전처리
- **불필요한 컬럼 제거** (`id`, `Unnamed: 32`)  
- **진단값 변환:** `B → 0`, `M → 1`  
- **이상치 처리:** 박스플롯, 히스토그램 활용  
- **Feature Selection:**  
  - **상관계수 분석**  
  - **트리 기반 모델의 Feature Importance 평가**  

## 🤖 모델 학습 및 평가
### ✅ 비교한 모델
- **트리 기반 모델:** Random Forest, Extra Trees, Gradient Boosting  
- **선형 모델:** SVM, Logistic Regression  

### 📈 성능 비교 (Accuracy)
| 모델 | 정확도 |
|------|------|
| **Extra Trees** | **97.37%** |
| Gradient Boosting | 95.61% |
| Random Forest | 95.61% |
| SVM | 95.61% |
| Logistic Regression | 96.49% |

> **결론:** Extra Trees 모델이 가장 높은 성능을 기록  
