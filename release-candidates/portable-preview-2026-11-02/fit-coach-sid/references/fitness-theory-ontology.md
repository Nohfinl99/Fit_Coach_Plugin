# fitness-theory-ontology.md — v1.1.0 interface / provenance

Role: Theory / mechanisms. Domain body nhập từ tài liệu người dùng ngày 2026-10-03; không phải medical/evidence review.

## Source status and evidence registry

Default status of the imported corpus is IMPORTED_UNVERIFIED; book attributions have not been checked against exact editions/pages. The single authoritative claim register is the Source-review register in sibling file `fitness-protocols.md`. EX-ID citations below are valid only when the corresponding row in that register is available and its scope matches the sentence. If the register is unavailable, treat the claim as IMPORTED_UNVERIFIED. This file explains theory; it does not independently authorize protocol or dose. Benchmark text is not scientific evidence.

## Imported domain corpus

# fitness-theory-ontology.md — Theoretical & Mechanistic Ontology (SID Fit Coach)

> **Authority:** Unified Production Knowledge Layer (Quad-File Architecture: File 2/4)  
> **Source Corpus:** K01–K16 Knowledge Decompositions  
> - *Science and Development of Muscle Hypertrophy (2nd Edition)* — Brad Schoenfeld  
> - *The Muscle and Strength Pyramid: Nutrition & Training* — Eric Helms, Andy Morgan, Andrea Valdez  
> **Phạm vi tài liệu:** Lý thuyết bản thể học (Ontology), Mạng lưới cơ chế sinh học (Biomechanical & Physiological Mechanisms), Các định lý quan hệ nhân quả (Causal Axioms), và Ranh giới khoa học (Scientific Boundaries).  
> **Ràng buộc kiến trúc:** Tách biệt tuyệt đối khỏi bảng protocol thực thi (Zero Action Tables — các bảng này thuộc về File 3/4: `fitness-protocols.md`).

---

# MỤC LỤC TỔNG QUAN HỆ THỐNG

- [PHẦN 1: TRỤC HUẤN LUYỆN & SINH CƠ (TRAINING & HYPERTROPHY ONTOLOGY — K01 ĐẾN K08)](#phần-1-trục-huấn-luyện--sinh-cơ-training--hypertrophy-ontology--k01-đến-k08)
  - [Module K01: Nền tảng Sinh lý Học của Sự Phì đại Cơ bắp (KN-PBH-01)](#module-k01-nền-tảng-sinh-lý-học-của-sự-phì-đại-cơ-bắp-kn-pbh-01)
  - [Module K02: Cơ chế Sinh học Phì đại & Ranh giới Nhân quả (KN-MHY-01)](#module-k02-cơ-chế-sinh-học-phì-đại--ranh-giới-nhân-quả-kn-mhy-01)
  - [Module K03: Bản thể học Đo lường & Đánh giá Tiến độ (KN-MPA-01)](#module-k03-bản-thể-học-đo-lường--đánh-giá-tiến-độ-kn-mpa-01)
  - [Module K04: Thang Phân cấp Biến số Tập luyện Kháng lực (KN-RTV-01, KN-RTV-02, KN-RTV-03)](#module-k04-thang-phân-cấp-biến-số-tập-luyện-kháng-lực-kn-rtv-01-kn-rtv-02-kn-rtv-03)
  - [Module K05: Cơ chế Kỹ thuật Nâng cao & Ranh giới Hiệu quả (KN-ATP-01)](#module-k05-cơ-chế-kỹ-thuật-nâng-cao--ranh-giới-hiệu-quả-kn-atp-01)
  - [Module K06: Huấn luyện Đồng thời & Hiện tượng Giao thoa Sinh lý (KN-ACT-01)](#module-k06-huấn-luyện-đồng-thời--hiện-tượng-giao-thoa-sinh-lý-kn-act-01)
  - [Module K07: Các Yếu tố Điều biến Cá thể Không Tất định (KN-IMH-01)](#module-k07-các-yếu-tố-điều-biến-cá-thể-không-tất-định-kn-imh-01)
  - [Module K08: Cơ sinh học Lập trình & Quản lý Phục hồi (KN-HPD-01, KN-HPD-02)](#module-k08-cơ-sinh-học-lập-trình--quản-lý-phục-hồi-kn-hpd-01-kn-hpd-02)
- [PHẦN 2: TRỤC DINH DƯỠNG & CHUYỂN HÓA (NUTRITION & METABOLISM ONTOLOGY — K09 ĐẾN K16)](#phần-2-trục-dinh-dưỡng--chuyển-hóa-nutrition--metabolism-ontology--k09-đến-k16)
  - [Module K09: Cân bằng Năng lượng & Động học Trọng lượng Cơ thể (KN-EBW-01, KN-EBW-02)](#module-k09-cân-bằng-năng-lượng--động-học-trọng-lượng-cơ-thể-kn-ebw-01-kn-ebw-02)
  - [Module K10: Động học Đại dưỡng chất & Vai trò Sinh lý (KN-MAF-01)](#module-k10-động-học-đại-dưỡng-chất--vai-trò-sinh-lý-kn-maf-01)
  - [Module K11: Vi dưỡng chất & Cân bằng Nội môi Thể dịch (KN-MIH-01)](#module-k11-vi-dưỡng-chất--cân-bằng-nội-môi-thể-dịch-kn-mih-01)
  - [Module K12: Thời điểm Nạp Dinh dưỡng & Động học Hồi phục Chuyển hóa (KN-NTF-01)](#module-k12-thời-điểm-nạp-dinh-dưỡng--động-học-hồi-phục-chuyển-hóa-kn-ntf-01)
  - [Module K13: Phân tầng Bằng chứng & Động học Thực phẩm Bổ sung (KN-SUP-01, KN-SUP-02)](#module-k13-phân-tầng-bằng-chứng--động-học-thực-phẩm-bổ-sung-kn-sup-01-kn-sup-02)
  - [Module K14: Sinh lý Giai đoạn Đỉnh cao & Ranh giới Nguy cơ Cắt cân (KN-CPW-01, KN-CPW-02)](#module-k14-sinh-lý-giai-đoạn-đỉnh-cao--ranh-giới-nguy-cơ-cắt-cân-kn-cpw-01-kn-cpw-02)
  - [Module K15: Phục hồi Nội tiết Sau Thi đấu & Chu kỳ hóa Dinh dưỡng (KN-PCR-01, KN-PCR-02)](#module-k15-phục-hồi-nội-tiết-sau-thi-đấu--chu-kỳ-hóa-dinh-dưỡng-kn-pcr-01-kn-pcr-02)
  - [Module K16: Tâm lý học Hành vi Ăn kiêng & Thần kinh Thể dịch Lối sống (KN-NBA-01, KN-NBA-02)](#module-k16-tâm-lý-học-hành-vi-ăn-kiêng--thần-kinh-thể-dịch-lối-sống-kn-nba-01-kn-nba-02)

---

# PHẦN 1: TRỤC HUẤN LUYỆN & SINH CƠ (TRAINING & HYPERTROPHY ONTOLOGY — K01 ĐẾN K08)

---

## Module K01: Nền tảng Sinh lý Học của Sự Phì đại Cơ bắp (KN-PBH-01)

### 1.1 Khung Khái niệm Cốt lõi (Conceptual Primitives)
- **Skeletal Muscle Architecture (Kiến trúc Cơ xương):** Hệ thống phân cấp cấu trúc từ toàn bộ bắp cơ (epimysium) $\rightarrow$ bó cơ (perimysium) $\rightarrow$ sợi cơ đơn lẻ (endomysium) $\rightarrow$ myofibril $\rightarrow$ sarcomere (đơn vị co cơ cơ bản chứa actin và myosin).
- **Motor Unit (Đơn vị Vận động):** Một tế bào thần kinh vận động alpha ($\alpha$-motor neuron) và toàn bộ các sợi cơ mà nó chi phối. Đơn vị vận động hoạt động theo nguyên lý "tất cả hoặc không" (All-or-None Principle).
- **Henneman's Size Principle (Nguyên lý Kích thước Henneman):** Các đơn vị vận động được huy động tuần tự từ nhỏ đến lớn (ngưỡng kích hoạt thấp $\rightarrow$ sợi Type I bền bỉ, tạo lực thấp; tiếp đến ngưỡng kích hoạt cao $\rightarrow$ sợi Type IIa và IIx tạo lực lớn, dễ mệt mỏi). Sự huy động đầy đủ các đơn vị vận động ngưỡng cao là điều kiện tiên quyết bắt buộc để kích hoạt phì đại ở các sợi cơ có tiềm năng tăng trưởng lớn nhất.
- **Myonuclear Domain Theory (Lý thuyết Miền Nhân tế bào Cơ):** Mỗi nhân tế bào cơ (myonucleus) chỉ quản lý quá trình phiên mã và tổng hợp protein trong một thể tích tế bào chất hữu hạn. Khi sợi cơ phì đại vượt qua ngưỡng giới hạn miền nhân, sự kích hoạt và dung hợp của Tế bào Vệ tinh (Satellite Cells) là bắt buộc để bổ sung nhân mới.
- **Protein Turnover Dynamics (Động học Chu chuyển Protein):** Trạng thái phì đại ròng ($\Delta \text{Muscle Mass}$) là kết quả tích phân theo thời gian của Cân bằng Protein Cơ bắp Ròng (Net Muscle Protein Balance - NPB):
  $$\text{NPB} = \text{MPS (Muscle Protein Synthesis)} - \text{MPB (Muscle Protein Breakdown)}$$
  $\Delta \text{Muscle Mass} > 0 \iff \text{MPS} > \text{MPB}$ trong một chu kỳ thời gian nhất định.

### 1.2 Mạng lưới Cơ chế Sinh học (Mechanistic Network)
- **Tín hiệu Thần kinh - Cơ:** Xung điện thần kinh $\rightarrow$ giải phóng Acetylcholine tại khe synap $\rightarrow$ khử cực màng sarcolemma $\rightarrow$ giải phóng $Ca^{2+}$ từ mạng lưới nội chất (sarcoplasmic reticulum) $\rightarrow$ gắn vào Troponin C $\rightarrow$ dịch chuyển Tropomyosin bộc lộ vị trí gắn kết Actin $\rightarrow$ Cầu nối ngang Myosin hình thành và tạo lực kéo (Power Stroke).
- **Con đường Truyền tín hiệu Phì đại Nội bào (Intracellular Signaling Pathways):**
  - **Trục Tín hiệu Trung tâm:** Biến dạng cơ học của màng tế bào $\rightarrow$ Kích hoạt thụ thể cơ học (Costamere, Integrin, Titin kinase) $\rightarrow$ Tổng hợp Phosphatidic Acid (PA) qua Phospholipase D và kích hoạt Focal Adhesion Kinase (FAK) $\rightarrow$ Kích hoạt phức hợp **mTORC1 (Mechanistic Target of Rapamycin Complex 1)** $\rightarrow$ Phosphoryl hóa p70S6K và ức chế 4E-BP1 $\rightarrow$ Khởi động dịch mã ribosome và sinh tổng hợp protein tơ cơ.
  - **Trục MAPK/ERK:** Phản ứng với biến dạng cơ học và stress chuyển hóa, điều hòa sự biểu hiện gen sinh trưởng và hoạt hóa tế bào vệ tinh.
  - **Trục Ức chế Sinh cơ:** Myostatin $\rightarrow$ Thụ thể ActRIIB $\rightarrow$ Kích hoạt Smad2/3 $\rightarrow$ Ức chế tổng hợp protein và ngăn chặn tế bào vệ tinh phân chia. Tập luyện kháng lực tạo ra sự ức chế biểu hiện myostatin nội sinh.
- **Hệ thống Nội tiết, Cận tiết & Tự tiết (Endocrine, Paracrine & Autocrine):**
  - *Cận tiết/Tự tiết (Local Factors):* IGF-1 cục bộ (Mechanogrowth Factor - MGF) được tổng hợp trực tiếp từ sợi cơ khi chịu sức căng, hoạt động tại chỗ để kích hoạt trục IGF-1/Akt/mTORC1 và kích thích tế bào vệ tinh.
  - *Nội tiết toàn thân (Systemic Hormones):* Biến động cấp tính của Testosterone, GH, IGF-1 tuần hoàn sau buổi tập KHÔNG phản ánh hoặc quyết định mức độ phì đại dài hạn của cơ bắp (tương quan yếu, không phải quan hệ nhân quả trực tiếp).

### 1.3 Mệnh đề Causal Axioms & Ranh giới Khoa học
- **Định lý PBH-01 (Điều kiện Tiên quyết Thần kinh):** Không thể có phì đại cơ ở một sợi cơ nếu sợi cơ đó không được huy động thần kinh (motor unit recruitment) và chịu tải cơ học.
- **Định lý PBH-02 (Tương quan Giả Nội tiết Cấp tính):** Đỉnh tăng hormone toàn thân cấp tính (acute systemic endocrine spikes) sau buổi tập không phải là động lực nhân quả gây phì đại cơ bắp dài hạn.
- **Ranh giới Khoa học (Epistemic Boundaries):**
  - Khoa học hiện đại bác bỏ giả thuyết cho rằng tăng cơ hoàn toàn phụ thuộc vào việc "bơm nồng độ hormone sau tập". Yếu tố quyết định là độ nhạy cảm của thụ thể androgen nội bào và tín hiệu cơ học tại chỗ.
  - Tăng sản sợi cơ (Hyperplasia - tăng số lượng sợi cơ) ở người vẫn còn là vấn đề gây tranh cãi và có bằng chứng rất hạn chế; đại đa số sự gia tăng thể tích cơ bắp ở người trưởng thành diễn ra thông qua Phì đại sợi cơ (Hypertrophy - phì đại tơ cơ theo chiều ngang hoặc chiều dài).

---

## Module K02: Cơ chế Sinh học Phì đại & Ranh giới Nhân quả (KN-MHY-01)

### 2.1 Ba Cơ chế Đề xuất & Phân loại Vai trò Nhân quả
1. **Sức căng Cơ học (Mechanical Tension) — [ĐỘNG LỰC NHÂN QUẢ DUY NHẤT ĐƯỢC XÁC LẬP VỮNG CHẮC]:**
   - Sự kéo căng và tạo lực của các sợi cơ chống lại ngoại lực kích hoạt thụ thể cơ học (mechanosensors).
   - Bao gồm Sức căng Chủ động (Active Tension do chu kỳ cầu nối actin-myosin tạo ra) và Sức căng Bị động (Passive Tension do sự kéo dãn các cấu trúc đàn hồi, chủ yếu là protein Titin).
   - Sức căng cơ học tối đa đạt được khi: Huy động tối đa đơn vị vận động + Tốc độ co cơ chậm lại do tải trọng nặng hoặc do mệt mỏi tích lũy (theo Mối quan hệ Lực - Vận tốc: Force-Velocity Relationship).
2. **Căng thẳng Chuyển hóa (Metabolic Stress) — [YẾU TỐ ĐIỀU BIẾN / HỖ TRỢ GIÁN TIẾP]:**
   - Sự tích tụ các chất chuyển hóa (ion $H^+$, lactate, vô cơ phosphate $P_i$, ADP) do phụ thuộc vào con đường đường phân kỵ khí khi cơ bắp bị thiếu oxy cục bộ (ischemia/hypoxia).
   - Cơ chế gián tiếp: Mệt mỏi chuyển hóa làm suy yếu các sợi cơ co chậm Type I $\rightarrow$ buộc hệ thần kinh phải kích hoạt bù trừ các đơn vị vận động Type II ngưỡng cao để duy trì lực $\rightarrow$ tạo sức căng cơ học lên các sợi Type II dù dùng tải trọng nhẹ.
   - Sưng tế bào (Cell Swelling): Tích tụ chất thẩm thấu làm nước tràn vào nội bào $\rightarrow$ tạo áp lực lên màng sarcolemma, có thể hoạt hóa thụ thể integrin như một tín hiệu kích thích tổng hợp protein bảo vệ cấu trúc tế bào.
3. **Tổn thương Cơ bắp (Muscle Damage / EIMD) — [HỆ QUẢ PHỤ / KHÔNG PHẢI ĐỘNG LỰC NHÂN QUẢ]:**
   - Vi rách cấu trúc sarcomere (Z-disc streaming), tổn thương màng sarcolemma và phản ứng viêm thứ cấp dẫn đến đau mỏi cơ khởi phát muộn (DOMS).
   - Bằng chứng khoa học xác lập: Tổn thương cơ bắp nghiêm trọng KHÔNG tỷ lệ thuận với mức độ phì đại cơ, thậm chí làm giảm khả năng tạo lực, cản trở việc tuyển mộ đơn vị vận động ở các buổi tập kế tiếp và lãng phí một phần lớn MPS chỉ để phục hồi sửa chữa mô thay vì tạo ra sự bồi đắp tơ cơ ròng (net contractile accretion).

### 2.2 Mệnh đề Causal Axioms & Ranh giới Ngộ nhận
- **Định lý MHY-01 (Axiom Sức căng Cơ học Tối thượng):** Sức căng cơ học là cơ chế sinh học cần và đủ để kích hoạt chuyển đổi tín hiệu cơ học thành sinh hóa (mechanotransduction) dẫn đến phì đại cơ bắp.
- **Định lý MHY-02 (Axiom Độc lập của Đau mỏi):** Đau cơ (DOMS) và cảm giác "bỏng rát" chuyển hóa (metabolic burn) là các hiện tượng sinh lý đi kèm, KHÔNG phải là thước đo của hiệu quả kích thích phì đại.
- **Ranh giới Khoa học (Epistemic Boundaries):**
  - *Chặn ngộ nhận "No Pain No Gain":* Việc cố tình tập luyện để phá hủy cơ bắp (excessive eccentric damage) chỉ làm tăng thời gian phục hồi và tăng nguy cơ chấn thương gân cơ mà không tạo thêm bất kỳ lợi thế phì đại nào.
  - Sưng cơ tức thì sau buổi tập (The Pump) là hiện tượng dịch chuyển thể dịch nội bào ngắn hạn (acute edema), không thể đồng nhất với sự gia tăng diện tích mặt cắt ngang sinh lý (physiological cross-sectional area - PCSA) của tơ cơ.

---

## Module K03: Bản thể học Đo lường & Đánh giá Tiến độ (KN-MPA-01)

### 3.1 Phân cấp Phương pháp Đo lường & Giới hạn Sai số
- **Cấp độ Nghiên cứu Lâm sàng (Laboratory Standards):**
  - *MRI & CT (Cộng hưởng từ & Cắt lớp vi tính):* Tiêu chuẩn vàng để đo PCSA và thể tích cơ bắp ($cm^3$). Độ chính xác cực cao, phân tách được mô cơ và mô mỡ nội bào, nhưng chi phí đắt đỏ và không khả thi cho theo dõi định kỳ.
  - *B-mode Ultrasound (Siêu âm cơ xương):* Đo độ dày cơ (muscle thickness) và góc bó cơ (pennation angle). Phản ánh tăng trưởng cục bộ chính xác, nhưng nhạy cảm với góc đặt đầu dò và hiện tượng sưng cơ sau tập (cần đo sau buổi tập ít nhất 48-72h).
  - *DEXA (Hấp thụ tia X kép):* Đo khối nạc không xương (Fat-Free Soft Tissue). Bị nhiễu mạnh bởi trạng thái hydrat hóa cơ thể, lượng glycogen tích trữ và cặn bã trong đường tiêu hóa.
- **Cấp độ Thực địa Ứng dụng (Field-Level Monitoring):**
  - *Cân nặng Cơ thể (Scale Bodyweight):* Đo lường biến thiên tổng khối lượng. Chứa độ nhiễu cực lớn do nước, muối, glycogen, chất thải và chu kỳ hormone.
  - *Thước dây nhân trắc (Circumferences):* Đo chu vi chi và các vòng cơ thể. Không thể phân biệt được giữa tăng cơ, tăng mỡ dưới da hay tích nước ngoại bào.
  - *Hiệu suất Tạ trong Giáo án (Training Logbook Performance):* Tăng mức tạ hoặc số reps ở cùng mức RIR/kỹ thuật chuẩn mực qua thời gian là chỉ số gián tiếp có độ tin cậy thực tiễn cao nhất chứng minh sự thích nghi cấu trúc cơ xương.

### 3.2 Động học Tách Nhiễu Khỏi Xu hướng (Noise-to-Signal Demarcation)
- **Snapshot (Điểm đo Đơn lẻ):** Mang giá trị thông tin tiệm cận zero đối với việc đánh giá phì đại hoặc mất mỡ. Một lần nhảy cân nặng đột ngột $\pm 1-2\text{ kg}$ trong 24 giờ phản ánh $100\%$ biến động cân bằng nước/glycogen hoặc phân trong trực tràng.
- **Trendline (Đường Xu hướng Trung bình Động):** Đánh giá dựa trên trung bình trượt 7 ngày (7-day moving average), so sánh giữa các tuần và đánh giá chu kỳ 2–4 tuần.
- **Quy tắc Đánh giá Đa biến (Multivariate Cross-Validation):** Tiến độ chỉ được xác nhận khi có sự đồng thuận từ ít nhất 2 trong 3 trục tín hiệu:
  1. *Trục Hiệu suất:* Mức tạ/reps tăng tiến ổn định với form chuẩn.
  2. *Trục Nhân trắc:* Số đo chu vi mục tiêu tăng/giảm phù hợp pha tập.
  3. *Trục Hình ảnh:* Độ nét cơ và tỷ lệ trực quan cải thiện qua ảnh chụp chuẩn hóa góc/ánh sáng sau mỗi 4–8 tuần.

---

## Module K04: Thang Phân cấp Biến số Tập luyện Kháng lực (KN-RTV-01, KN-RTV-02, KN-RTV-03)

### 4.1 Thang Phân cấp Ưu tiên Biến số (Variable Hierarchy)
```text
CẤP 1: CƯỜNG ĐỘ GẮNG SỨC (INTENSITY OF EFFORT / PROXIMITY TO FAILURE)
   └── Chọn effort theo mục tiêu, bài tập và khả năng kiểm soát; RIR là ước lượng
CẤP 2: KHỐI LƯỢNG TẬP LUYỆN (VOLUME: HARD SETS)
   └── Số hiệp tập hiệu quả tiệm cận ngưỡng thất bại trong tuần
CẤP 3: TẦN SUẤT & PHÂN BỔ (FREQUENCY & DISTRIBUTION)
   └── Tối ưu hóa chất lượng từng hiệp và tốc độ tổng hợp protein
CẤP 4: BIÊN ĐỘ VẬN ĐỘNG & LỰA CHỌN BÀI TẬP (ROM & EXERCISE SELECTION)
   └── Kéo căng cơ có tải, bài tập phù hợp cấu trúc cơ thể
CẤP 5: THỜI GIAN NGHỈ & NHỊP ĐỘ (REST INTERVALS & TEMPO)
   └── Phục hồi mệt mỏi thần kinh trung ương và kiểm soát gia tốc
```

### 4.2 Bản thể học Chi tiết từng Biến số
- **Cường độ Tải trọng (Load / %1RM) & Phổ Lặp lại (Repetition Spectrum):**
  - *Phổ tải và mục tiêu:* ACSM 2026 (EX-11) xác định tải nặng (≥80% 1RM) là một biến có lợi cho sức mạnh. Với hypertrophy, các mức tải thấp đến cao không cho khác biệt nhất quán trong tổng quan này. Đây không phải bằng chứng mọi mức tải đều tương đương tuyệt đối; hiệu quả phụ thuộc protocol, effort, population và cách so volume.
  - *Đặc tính Đánh đổi:*
    - Phổ rep/tải cụ thể còn lệ thuộc mục tiêu, bài và người tập. Những “sweet spot” và tỷ lệ volume phân bổ trong bảng protocol là imported guidance, chưa được EX-11 phê duyệt thành quy tắc cá nhân.
- **Cường độ Gắng sức (Proximity to Failure: RIR / RPE):**
  - *Khái niệm RIR (Reps in Reserve):* Số lần lặp lại dự trữ trước khi đạt điểm thất bại đồng tâm cơ học (concentric failure).
  - *Proximity to failure:* Không xem “effective reps”, slowdown hay huy động 100% sợi cơ như ngưỡng đã xác lập cho mọi bài/người. Dùng đồng thời hai loại kết quả: EX-04 không tìm thấy ưu thế rõ khi so momentary failure với non-failure theo nhóm; phân tích liên tục exploratory EX-10 gợi ý hypertrophy tăng khi dừng gần failure hơn. EX-10 suy RIR từ mô tả chương trình, fit mô hình khiêm tốn và không xác định một RIR tối ưu chính xác. EX-11 cũng không thấy tập đến fatigue/failure ảnh hưởng nhất quán các outcome hypertrophy.
- **Khối lượng Tập luyện (Volume — Hard Sets):**
  - EX-11 ủng hộ higher weekly volume (≥10 sets/week) như một tín hiệu dose-response trung bình cho hypertrophy ở healthy adults. Con số này không xác lập MEV/MAV/MRV cá nhân, ngưỡng “junk volume” hoặc quota bắt buộc cho từng nhóm cơ. Các đường cong và range chi tiết bên dưới corpus vẫn IMPORTED_UNVERIFIED nếu không có row riêng.
- **Tần suất Tập luyện (Frequency):**
  - Tần suất đóng vai trò như một **công cụ phân phối khối lượng** (volume delivery tool).
  - Với hypertrophy khi volume được cân bằng, EX-11 không thấy tần suất từ 1 buổi đến >5 buổi/tuần tạo khác biệt nhất quán. Tần suất vẫn có thể dùng để phân phối buổi/khối lượng theo thời gian và khả năng tuân thủ; không tuyên bố một ngưỡng chia buổi bắt buộc hay lợi ích MPS nhân đôi.
  - Với sức mạnh, EX-11 ghi nhận ≥2 sessions/week là biến có lợi trong tổng hợp. Áp dụng theo goal, lịch và population; không biến thành chỉ định lịch duy nhất.
- **Biên độ Vận động (Range of Motion - ROM):**
  - *ROM và chiều dài cơ:* EX-01/02 là các trial cụ thể trên seated leg curl và overhead elbow extension; EX-05 so lengthened partial với full ROM ở arm flexors/extensors. Meta-analysis EX-09 ghi nhận khác biệt vùng hypertrophy rất nhỏ giữa các điều kiện mean muscle length dài/ngắn, với chênh lệch chiều dài trung bình giữa điều kiện hạn chế. Không suy ra “cơ dài hơn luôn tăng nhiều hơn”, cũng không dùng EX-09 để khẳng định mọi bài/ROM tương đương. Với sức mạnh, EX-11 ủng hộ complete ROM trong tổng hợp healthy adults.
  - *Giới hạn cơ chế:* Các hypertrophy outcomes này không tự xác minh titin hoặc sarcomerogenesis là nguyên nhân. Cần nguồn cơ chế riêng trước khi kết luận.
- **Thời gian Nghỉ giữa Hiệp (Rest Intervals):**
  - Nghỉ dài ($\ge 2$ phút, thậm chí $3-5$ phút đối với bài tập phức hợp đa khớp) tạo ra phì đại cơ bắp LỚN HƠN so với nghỉ ngắn ($\le 60$ giây).
  - *Cơ chế:* Nghỉ quá ngắn không đủ thời gian để hệ thần kinh trung ương hồi phục khả năng dẫn truyền xung lực và không đủ tái tạo phosphocreatine $\rightarrow$ làm giảm sản sinh lực ở hiệp kế tiếp $\rightarrow$ giảm sức căng cơ học lên các đơn vị vận động Type II.
- **Nhịp độ Co cơ (Tempo):**
  - Meta-analysis EX-03 ghi nhận hypertrophy tương tự trong dải tổng thời gian rep 0.5–8 giây ở điều kiện nghiên cứu. Đây không phải thời lượng riêng eccentric và không tạo tempo bắt buộc. Dùng nhịp có kiểm soát theo bài/mục tiêu; claim bảo vệ khớp/gân cần nguồn riêng.


---

## Module K05: Cơ chế Kỹ thuật Nâng cao & Ranh giới Hiệu quả (KN-ATP-01)

### 5.1 Các Kỹ thuật Nâng cao & Đánh giá Đánh đổi Sinh lý
1. **Drop Sets & Strip Sets:**
   - *Bản chất:* Thực hiện hiệp tập đến ngưỡng thất bại, ngay lập tức giảm tải $20-25\%$ và tiếp tục tập tiếp không nghỉ.
   - *Cơ chế:* Duy trì trạng thái huy động đơn vị vận động Type II đã được kích hoạt từ hiệp trước trong khi tiết kiệm thời gian.
   - *Đánh đổi:* Mức độ phì đại tương đương với hiệp tập truyền thống nếu volume-equated; chi phí mệt mỏi chuyển hóa cao; thích hợp cho bài tập cô lập (isolation), chống chỉ định trên bài phức hợp trục cột sống (axial loading).
2. **Rest-Pause Training & Myo-reps:**
   - *Bản chất:* Thực hiện hiệp kích hoạt ($10-12$ reps đến $1-2$ RIR), nghỉ ngắn $10-15$ giây (khoảng $3-5$ nhịp thở sâu), sau đó thực hiện các cụm nhỏ $3-5$ reps liên tiếp.
   - *Cơ chế:* Loại bỏ các "reps khởi động không hiệu quả" ở đầu hiệp, tối đa hóa mật độ reps hiệu quả (effective reps density) trên đơn vị thời gian.
   - *Đánh đổi:* Hiệu quả thời gian cực cao; chi phí mệt mỏi thần kinh tăng nhanh; cần kiểm soát chặt chẽ kỹ thuật để tránh sụp đổ form.
3. **Supersets & Antagonist Paired Sets (APS):**
   - *Bản chất:* Ghép 2 bài tập của các nhóm cơ đối vận (ví dụ: Biceps gập tay + Triceps duỗi tay) hoặc hai nhóm cơ không liên quan (ví dụ: Bench Press + Calves) xen kẽ nhau với thời gian nghỉ ngắn giữa hai bài.
   - *Cơ chế:* Hiện tượng ức chế tương hỗ (reciprocal inhibition) có thể giúp cơ đối vận hồi phục tốt hơn và tăng nhẹ sản lượng lực; tăng gấp đôi mật độ buổi tập.
   - *Đánh đổi:* Không làm giảm hiệu suất nếu ghép cơ đối vận/không liên quan; nhưng nếu ghép 2 bài cùng một nhóm cơ (Pre-exhaustion/Post-exhaustion) sẽ làm giảm mức tải ở bài thứ hai do mệt mỏi cục bộ.
4. **Loaded Stretch Training (Kéo căng Dưới tải):**
   - *Bản chất:* Giữ tĩnh hoặc nhấn sâu ở vị trí cơ bắp bị kéo căng cực đại khi kết thúc hiệp tập.
   - *Cơ chế:* Tận dụng sức căng cơ học thụ động tối đa và cơ chế thiếu máu cục bộ gây sưng tế bào.
   - *Đánh đổi:* Bằng chứng còn hỗn hợp; nguy cơ tổn thương mô liên kết nếu khớp không ổn định.

### 5.2 Định lý Phân định Kỹ thuật Nâng cao
- **Định lý ATP-01 (Định lý Tiết kiệm Thời gian):** Các kỹ thuật nâng cao (Drop set, Rest-pause, Supersets) là **công cụ tối ưu hóa hiệu quả thời gian (time-efficiency tools)**, KHÔNG PHẢI là phương pháp kích thích phì đại vượt trội hơn so với các hiệp tập truyền thống được nghỉ ngơi đầy đủ.

---

## Module K06: Huấn luyện Đồng thời & Hiện tượng Giao thoa Sinh lý (KN-ACT-01)

### 6.1 Cơ chế Phân tử của Hiện tượng Giao thoa (The Interference Effect)
- **Xung đột Con đường Tín hiệu Tế bào:**
  - Tập luyện Sức mạnh/Phì đại $\rightarrow$ Kích hoạt trục **Akt $\rightarrow$ mTORC1** $\rightarrow$ Sinh tổng hợp Protein sợi cơ.
  - Tập luyện Hiếu khí (Cardio kéo dài, cường độ cao) $\rightarrow$ Tăng tỷ lệ AMP/ATP $\rightarrow$ Kích hoạt enzyme **AMPK (AMP-activated protein kinase)** và **SIRT1 $\rightarrow$ PGC-1$\alpha$** $\rightarrow$ Kích thích sinh tổng hợp ty thể và tăng oxy hóa acid béo.
  - *Điểm xung đột:* AMPK trực tiếp phosphoryl hóa và ức chế phức hợp Raptor trong mTORC1, đồng thời kích hoạt TSC2 để dập tắt tín hiệu tăng trưởng cơ bắp.
- **Xung đột Thần kinh - Cơ và Mệt mỏi Dư lượng (Residual Fatigue):**
  - Cardio làm cạn kiệt glycogen sợi cơ, gây tổn thương cấu trúc do chấn động lặp lại (đặc biệt là chạy bộ - high impact eccentric pounding) $\rightarrow$ làm suy giảm khả năng phát lực tối đa và chất lượng của buổi tập tạ sau đó.

### 6.2 Các Đòn bẩy Giảm thiểu Giao thoa (Interference Mitigation Axioms)
1. **Lựa chọn Hình thức (Modality Selection):**
   - Đạp xe (Cycling), Chèo thuyền (Rowing), Đi bộ dốc (Incline Walking) tạo ra ít giao thoa hơn đáng kể so với Chạy bộ (Running).
   - *Lý do:* Chạy bộ có pha tiếp đất cưỡng bức (eccentric impact) gây tổn thương cơ bắp và mệt mỏi gân khớp; trong khi đạp xe chủ yếu là co cơ đồng tâm (concentric-dominant), có kiểu hình tuyển mộ cơ khớp tương đồng hơn với chuyển động squat/leg press.
2. **Khoảng cách Thời gian (Temporal Spacing):**
   - Phân tách buổi tập tạ và buổi cardio ít nhất **6 đến 24 giờ** để cho phép nồng độ AMPK nội bào hạ xuống và glycogen được bù đắp một phần.
   - Nếu bắt buộc phải tập chung một buổi: Luôn tập tạ TRƯỚC, tập cardio SAU.
3. **Liều lượng và Cường độ (Dose & Intensity):**
   - Cardio cường độ thấp ổn định (LISS - Low-Intensity Steady State / Zone 2) ít gây xung đột tín hiệu và dễ kiểm soát mệt mỏi hơn HIIT khi tổng khối lượng tập tạ trong tuần đã ở mức cao.

---

## Module K07: Các Yếu tố Điều biến Cá thể Không Tất định (KN-IMH-01)

### 7.1 Mạng lưới Biến số Điều biến Nội tại
- **Kinh nghiệm Tập luyện (Training Status & Ceiling Effect):**
  - *Tân binh (Untrained / Novice):* Tiềm năng thích nghi cực lớn; bất kỳ kích thích nào từ $30\%$ 1RM cũng gây phì đại; thích nghi thần kinh chiếm ưu thế trong 4–8 tuần đầu; tốc độ tăng cơ có thể đạt $1-1.5\%$ trọng lượng cơ thể/tháng.
  - *Trung cấp (Intermediate):* Tốc độ tăng trưởng chậm dần; đòi hỏi tính hệ thống về volume và kỹ thuật bài tập; MPS diễn ra ngắn hơn (thu hẹp từ 48-72h xuống còn 12-24h).
  - *Nâng cao (Advanced):* Tiệm cận trần giới hạn di truyền; tốc độ tăng cơ chậm lại ở mức vài trăm gram mỗi năm; đòi hỏi chu kỳ hóa phức tạp và quản lý mệt mỏi cực kỳ chi tiết.
- **Tuổi tác & Kháng Đồng hóa (Age & Anabolic Resistance):**
  - Người lớn tuổi (Sarcopenia / Master athletes) gặp hiện tượng Kháng Đồng hóa: Cùng một lượng kích thích cơ học hoặc cùng một lượng protein nạp vào tạo ra mức tăng MPS thấp hơn so với người trẻ.
  - *Cơ chế:* Giảm tưới máu mao mạch cơ, suy giảm độ nhạy insulin, giảm số lượng tế bào vệ tinh và viêm mãn tính mức độ thấp. Cần ngưỡng Leucine cao hơn và thời gian phục hồi giữa các buổi lâu hơn.
- **Giới tính Sinh học (Biological Sex):**
  - *Mức độ Tăng trưởng Tương đối:* Nam và nữ giới có **tỷ lệ phì đại cơ bắp tương đối ($\% \Delta \text{CSA}$) hoàn toàn tương đương nhau** khi tham gia cùng một chương trình tập luyện kháng lực.
  - *Khác biệt Tuyệt đối:* Nam giới có diện tích sợi cơ và tổng khối cơ ban đầu lớn hơn do nồng độ testosterone nội sinh lưu hành cao hơn gấp 10–15 lần từ giai đoạn dậy thì.
  - *Khả năng Chịu mệt mỏi ở Nữ:* Nữ giới sở hữu tỷ lệ sợi cơ Type I cao hơn, tưới máu cơ tốt hơn và nồng độ estrogen bảo vệ màng tế bào $\rightarrow$ có khả năng chịu đựng thể tích tập cao hơn, hồi phục nhanh hơn giữa các hiệp và chịu mệt mỏi cơ bắp tốt hơn nam giới.
- **Biến thiên Di truyền (Inter-Individual Variability - Responders Spectrum):**
  - Sự khác biệt về cấu trúc thụ thể androgen, số lượng tế bào vệ tinh nền, khả năng sinh học của ribosome (ribosome biogenesis) và nồng độ myostatin tạo ra phổ phản ứng: Low-responders vs High-responders.
  - Không có giáo án nào là tối ưu tuyệt đối cho tất cả mọi cá nhân.

---

## Module K08: Cơ sinh học Lập trình & Quản lý Phục hồi (KN-HPD-01, KN-HPD-02)

### 8.1 Cơ sinh học Ứng dụng trong Tuyển chọn Bài tập
- **Resistance Profile vs Strength Curve (Biểu đồ Kháng lực & Đường cong Sức mạnh):**
  - *Đường cong Sức mạnh:* Khả năng tạo lực của cơ bắp biến thiên theo góc khớp (ngắn nhất, trung bình, dài nhất) do cánh tay đòn nội (internal moment arm) và mức độ chồng chéo actin-myosin (chiều dài sarcomere).
  - *Biểu đồ Kháng lực:* Ngoại lực tác động (mô-men kháng lực ngoại = Lực $\times$ Cánh tay đòn ngoại) thay đổi liên tục trong suốt quỹ đạo chuyển động.
  - *Nguyên tắc Tối ưu Hóa:* Bài tập mang lại hiệu quả phì đại cao nhất khi Biểu đồ Kháng lực khớp với Đường cong Sức mạnh của cơ mục tiêu, và tạo ra thử thách lớn nhất ở vị trí cơ bắp bị kéo căng (stretched position).
- **Mặt phẳng Chuyển động & Căn chỉnh Hướng Sợi cơ (Fiber Alignment):**
  - Khớp quỹ đạo chuyển động của tạ với góc hướng của bó sợi cơ giải phẫu (ví dụ: chia nhánh ngực đòn, ngực ức, ngực sườn; hoặc các nhánh deltoid) để tối đa hóa cánh tay đòn nội của nhóm cơ chủ vận và giảm thiểu sự bù trừ của các nhóm cơ phụ.

### 8.2 Tỷ lệ Kích thích trên Mệt mỏi (Stimulus-to-Fatigue Ratio - SFR)
- **Định nghĩa SFR:** Tỷ số giữa tín hiệu phì đại thu được (sự huy động đơn vị vận động, sức căng cơ học, cảm nhận cơ bắp) so với cái giá mệt mỏi phải trả (mệt mỏi thần kinh trung ương, áp lực lên gân khớp, tổn thương mô liên kết, DOMS kéo dài).
- **Tiêu chí Bài tập có SFR Cao:**
  - Tạo sức căng cơ học lớn trực tiếp lên nhóm cơ đích.
  - Dễ dàng kiểm soát kỹ thuật và duy trì sự ổn định (stability) cao.
  - Ít gây mỏi thần kinh toàn thân và không làm đau/áp lực bệnh lý lên các khớp lân cận.
  - Ví dụ: Chest-supported Dumbbell Row có SFR cho cơ lưng cao hơn Barbell Bent-over Row do giải phóng cơ dựng gai sống và khớp háng khỏi việc giữ ổn định trục cột sống.

### 8.3 Bản thể học Quản lý Khối lượng & Phục hồi (Volume Landmarks)
- **Thuật ngữ volume landmark (model nhập khẩu):** MV, MEV, MAV và MRV là nhãn huấn luyện dùng để mô tả volume duy trì, điểm bắt đầu tạo thích nghi, vùng volume có thể tiếp tục tạo thích nghi và giới hạn phục hồi ước tính. Chúng không phải ngưỡng sinh học đo trực tiếp hay mốc chuẩn hóa cho mọi người. Các khoảng số trong protocol corpus — gồm 4–6, 6–10, 12–20 và 20–25+ sets/nhóm cơ/tuần — vẫn `IMPORTED_UNVERIFIED` nếu không có row riêng trong evidence register; không dùng chúng như quota, mục tiêu tối ưu hoặc ngưỡng chẩn đoán.
- **Đọc tín hiệu volume và phục hồi:** Diễn giải volume cùng xu hướng hiệu suất, mức nỗ lực, đau, giấc ngủ, stress, lịch tập và khả năng tuân thủ. Một biến động đơn lẻ không chứng minh người tập đã vượt MRV hoặc cần deload. EX-11 hỗ trợ higher weekly volume (≥10 sets/week) như một tín hiệu trung bình ở healthy adults; không xác nhận landmark cá nhân hay kết luận rằng vượt một con số cụ thể gây overtraining.
- **Mệt mỏi và thời gian hồi phục:** Mệt mỏi ngoại vi và trung ương là các khái niệm sinh lý có thể góp phần vào suy giảm hiệu suất, nhưng không suy ra rằng mọi nhóm cơ hồi phục trong 24–48 giờ, mọi mệt mỏi ảnh hưởng toàn thân, hoặc CNS fatigue tự động đòi hỏi deload. Thời lượng và ngưỡng deload cố định trong corpus chưa được xác nhận bởi evidence register; điều chỉnh chỉ khi tín hiệu lặp lại và bối cảnh hỗ trợ quyết định đó.
---

# PHẦN 2: TRỤC DINH DƯỠNG & CHUYỂN HÓA (NUTRITION & METABOLISM ONTOLOGY — K09 ĐẾN K16)

---

## Module K09: Cân bằng Năng lượng & Động học Trọng lượng Cơ thể (KN-EBW-01, KN-EBW-02)

### 9.1 Định luật Nhiệt động Lực học & Phương trình Năng lượng
- **Định luật Thứ nhất Nhiệt động Lực học Ứng dụng:** Năng lượng không tự nhiên sinh ra hay mất đi, chỉ chuyển hóa từ dạng này sang dạng khác.
  $$\Delta \text{Năng lượng Tích trữ Nội tại} = \text{Năng lượng Nạp vào (EI)} - \text{Tổng Tiêu hao Năng lượng (TDEE)}$$
- **Bản thể học Các Thành phần của TDEE (Total Daily Energy Expenditure):**
  1. **BMR (Basal Metabolic Rate - Năng lượng Chuyển hóa Cơ bản):** Chiếm $60-70\%$ TDEE. Chi phí duy trì các chức năng tế bào sống tối thiểu ở trạng thái nghỉ hoàn toàn. Tỷ lệ thuận với khối lượng nạc (LBM).
  2. **TEF (Thermic Effect of Food - Hiệu ứng Nhiệt của Thức ăn):** Chiếm $8-10\%$ TDEE. Năng lượng tiêu hao để tiêu hóa, hấp thu và chuyển hóa chất dinh dưỡng.
     - *Protein:* $20-30\%$ (cao nhất).
     - *Carbohydrates:* $5-10\%$.
     - *Fats:* $0-3\%$ (thấp nhất).
  3. **EAT (Exercise Activity Thermogenesis - Tiêu hao Vận động Tập luyện):** Chiếm $5-10\%$ TDEE. Biến thiên theo cường độ và thời lượng tập luyện có cấu trúc.
  4. **NEAT (Non-Exercise Activity Thermogenesis - Tiêu hao Hoạt động Ngoài tập luyện):** Chiếm $15-30\%$ TDEE. Thành phần biến thiên mạnh nhất và dễ bị ức chế nhất khi cơ thể bị bỏ đói (đi bộ, đứng, cựa quậy, duy trì tư thế).

### 9.2 Thích nghi Chuyển hóa (Adaptive Thermogenesis)
- Khi rơi vào trạng thái thâm hụt năng lượng kéo dài, cơ thể kích hoạt cơ chế sinh tồn để giảm thiểu tiêu hao:
  - BMR sụt giảm mạnh hơn mức có thể dự đoán dựa trên sự mất mát khối lượng mô đơn thuần.
  - NEAT bị dập tắt vô thức: Giảm các cử động vi mô, cảm giác lười vận động tăng vọt.
  - Leptin, hormone tuyến giáp ($T_3$), Testosterone giảm mạnh; Cortisol và Ghrelin tăng vọt $\rightarrow$ tăng cảm giác đói dữ dội và giảm tốc độ oxy hóa chất béo.

### 9.3 Tỷ lệ Phân chia Dưỡng chất (P-Ratio / Partitioning Ratio) & Tốc độ Thay đổi Cân nặng
- **Khái niệm P-Ratio:** Tỷ lệ giữa protein cơ bắp và mỡ trong tổng khối lượng mô được tích lũy (khi thặng dư) hoặc bị phân giải (khi thâm hụt).
- **Yếu tố Quyết định P-Ratio:** Tỷ lệ mỡ cơ thể ban đầu (Body fat percentage), tập luyện kháng lực đủ tải, lượng protein nạp vào, nồng độ hormone sinh dục và di truyền.
- **Ranh giới Tốc độ Thay đổi Trọng lượng Khuyến nghị:**
  - *Tăng cơ (Bulking/Surplus):* Tốc độ tăng cân tối ưu chỉ nên dao động từ $0.25\%$ đến $0.5\%$ trọng lượng cơ thể/tuần đối với người mới/trung cấp, và $<0.25\%$/tuần đối với người nâng cao để hạn chế tích lũy mô mỡ thừa.
  - *Giảm mỡ (Cutting/Deficit):* Tốc độ giảm cân bền vững bảo toàn tối đa khối nạc là $0.5\%$ đến $1.0\%$ trọng lượng cơ thể/tuần. Giảm vượt quá $1.0\%$/tuần làm tăng vọt nguy cơ dị hóa cơ bắp và rối loạn nội tiết.
- **Bản thể học Tái cấu trúc Cơ thể (Body Recomposition):**
  - Khả năng đồng thời tăng cơ và giảm mỡ tại cùng một mốc thời gian là hiện tượng khoa học ĐÃ ĐƯỢC CHỨNG MINH.
  - *Điều kiện khả thi:* Người mới tập kháng lực, người quay lại sau thời gian dài bỏ tập (muscle memory), người thừa cân/béo phì (lượng mỡ dự trữ dồi dào cung cấp năng lượng cho quá trình đồng hóa), hoặc người sử dụng chất kích thích đồng hóa.

---

## Module K10: Động học Đại dưỡng chất & Vai trò Sinh lý (KN-MAF-01)

### 10.1 Kim tự tháp Ưu tiên Dinh dưỡng Eric Helms (Nutrition Pyramid Hierarchy)
```text
CẤP 1: CÂN BẰNG NĂNG LƯỢNG (ENERGY BALANCE / CALORIES)
   └── Quyết định hướng biến thiên trọng lượng cơ thể
CẤP 2: PHÂN BỔ ĐẠI DƯỠNG CHẤT & CHẤT XƠ (MACRONUTRIENTS & FIBER)
   └── Quyết định tỷ lệ nạc/mỡ (P-ratio) và hiệu suất vận động
CẤP 3: VI DƯỠNG CHẤT & NƯỚC (MICRONUTRIENTS & WATER)
   └── Bảo đảm sức khỏe tế bào, chức năng enzyme và nội môi
CẤP 4: THỜI ĐIỂM BỮA ĂN (NUTRIENT TIMING & FREQUENCY)
   └── Tối ưu hóa chu kỳ đồng hóa và phục hồi hiệu suất
CẤP 5: THỰC PHẨM BỔ SUNG (SUPPLEMENTATION)
   └── Lợi ích biên bổ trợ sau khi 4 cấp nền tảng đã vững chắc
```

### 10.2 Động học Protein & Phản ứng Sinh tổng hợp Cơ bắp (MPS)
- **Vai trò Sinh lý:** Cung cấp các acid amin thiết yếu (EAA) để xây dựng cấu trúc mô cơ, enzyme và hormone peptide.
- **Ngưỡng Leucine & Hiệu ứng Cơ bắp No (Muscle Full Effect):**
  - Acid amin Leucine đóng vai trò như chiếc chìa khóa kích hoạt công tắc mTORC1.
  - *Ngưỡng Leucine (Leucine Trigger):* Cần nạp tối thiểu xấp xỉ **$2.5 - 3.0\text{ g}$ Leucine** trong một bữa ăn (tương đương $25-40\text{ g}$ protein chất lượng cao tùy nguồn) để kích hoạt MPS đạt đỉnh cực đại.
  - *Muscle Full Effect:* Sau khi MPS được kích thích và đạt đỉnh sau $90-120$ phút, nồng độ MPS sẽ tự động rơi về đường cơ sở mặc dù nồng độ acid amin trong máu vẫn ở mức cao. Việc nạp thêm liên tục protein trong cửa sổ này không làm tăng thêm MPS.
- **Khung Nạp Đạm Toàn diện (Protein Dosing Continuum):**
  - *Mức tối ưu chung:* **$1.6 - 2.2\text{ g/kg}$ trọng lượng cơ thể/ngày** đáp ứng hoàn toàn nhu cầu đồng hóa tối đa cho đại đa số người tập kháng lực.
  - *Mức bảo vệ trong Thâm hụt Nặng / Gầy sắc nét:* Khi mỡ cơ thể rất thấp và mức thâm hụt năng lượng sâu, nhu cầu đạm có thể tăng lên **$2.3 - 3.1\text{ g/kg}$ khối lượng nạc (LBM)/ngày** để chống lại sự dị hóa mô cơ do thiếu cơ chất năng lượng.

### 10.3 Chuyển hóa Carbohydrate & Động học Glycogen
- **Cơ chất Ưu tiên cho Tập luyện Kháng lực:** Hoạt động co cơ cường độ cao phụ thuộc hoàn toàn vào quá trình đường phân kỵ khí (anaerobic glycolysis) sử dụng glucose nội bào và glycogen trong cơ.
- **Bảo toàn Cơ bắp Gián tiếp (Protein-Sparing Effect):** Khi carbohydrate được cung cấp đầy đủ, cơ thể không cần phải phân giải acid amin qua con đường tân tạo đường (gluconeogenesis) tại gan để cung cấp glucose cho não và hồng cầu.
- **Tích trữ Glycogen & Thể tích Sợi cơ:** Mỗi gram glycogen tích lũy trong cơ bắp kéo theo khoảng $3 - 4\text{ g}$ nước nội bào, góp phần tăng đường kính sợi cơ và duy trì trạng thái hydrat hóa tế bào thuận lợi cho tín hiệu đồng hóa.

### 10.4 Chất béo Cốt lõi & Ranh giới Nội tiết (Fat Baseline)
- **Vai trò Tối quan trọng:** Cấu tạo màng tế bào (phospholipid bilayer), hấp thu các vitamin tan trong dầu (A, D, E, K) và làm tiền chất tổng hợp hormone steroid sinh dục (Testosterone, Estrogen, Progesterone).
- **Ranh giới Sàn Tối thiểu (Essential Fat Floor):**
  - Nạp chất béo KHÔNG NÊN rơi xuống dưới **$0.5\text{ g/kg}$ thể trọng/ngày** hoặc thấp hơn **$15 - 20\%$ tổng năng lượng nạp vào** trong thời gian dài.
  - *Hậu quả khi tụt dưới sàn:* Sụt giảm nghiêm trọng nồng độ testosterone tự do, rối loạn kinh nguyệt ở nữ giới (mất kinh cơ năng do hạ đồi - FHA), suy giảm miễn dịch và khô khớp.

### 10.5 Chất xơ & Sức khỏe Đường ruột (Dietary Fiber)
- Phân loại: Chất xơ hòa tan (tạo gel, làm chậm rỗng dạ dày, tăng cảm giác no) và chất xơ không hòa tan (tăng khối lượng phân, kích thích nhu động ruột).
- Ngưỡng tối ưu: $10 - 15\text{ g}$ chất xơ trên mỗi $1000\text{ kcal}$ tiêu thụ (hoặc trung bình $25 - 40\text{ g/ngày}$). Quá ít gây táo bón và rối loạn vi sinh vật đường ruột; quá nhiều ($>50-60\text{ g/ngày}$) gây đầy hơi, cản trở hấp thu khoáng chất và làm giảm lượng ăn cần thiết trong giai đoạn tăng cân.

---

## Module K11: Vi dưỡng chất & Cân bằng Nội môi Thể dịch (KN-MIH-01)

### 11.1 Bản thể học Vi chất & Đa dạng Thực phẩm
- Vi chất dinh dưỡng (Vitamins & Minerals) không mang giá trị calo nhưng là các co-factor bắt buộc cho các phản ứng hóa sinh, dẫn truyền thần kinh, co cơ và chuyển hóa năng lượng tế bào.
- **Quy tắc Ưu tiên Thực phẩm Toàn phần (Whole Foods First):** Việc ăn uống đa dạng các nhóm màu sắc thực phẩm, rau củ quả, nguồn đạm phong phú luôn vượt trội hơn việc chỉ ăn thực đơn đơn điệu rồi dùng viên multivitamin tổng hợp, nhờ vào sự hiện diện của các hợp chất sinh học (phytonutrients) và khả năng hấp thu cộng hưởng sinh khả dụng cao.
- **Các Vi chất Thường gặp Rủi ro Thiếu hụt khi Ăn kiêng Khắc nghiệt:** Sắt (Iron - đặc biệt ở nữ vận động viên), Kẽm (Zinc), Canxi (Calcium), Vitamin D (tổng hợp nội tiết), và Vitamin B12 (ở người ăn thuần chay).

### 11.2 Cân bằng Nội môi Thể dịch & Điện giải (Fluid & Electrolyte Homeostasis)
- **Tác động của Thiếu nước (Hypohydration):**
  - Mất nước vượt quá **$2\%$ trọng lượng cơ thể** dẫn đến suy giảm có ý nghĩa thống kê về hiệu suất sức mạnh, số reps thực hiện trước khi thất bại và tăng mức độ căng thẳng nhiệt nội tại.
  - Thiếu nước làm giảm thể tích huyết tương $\rightarrow$ giảm thể tích nhát bóp tim $\rightarrow$ nhịp tim tăng vọt để bù trừ $\rightarrow$ suy giảm tưới máu đến các cơ bắp đang hoạt động.
- **Hệ thống Điện giải Vận động:**
  - *Natri ($Na^+$):* Cation ngoại bào chính. Đóng vai trò then chốt trong việc duy trì áp suất thẩm thấu thể dịch, thể tích máu và dẫn truyền điện thế hoạt động thần kinh cơ. Bắt buộc để hấp thu glucose ở ruột non thông qua chất đồng vận chuyển SGLT-1.
  - *Kali ($K^+$):* Cation nội bào chính. Phối hợp với bơm $Na^+/K^+$-ATPase duy trì điện thế nghỉ màng tế bào và quá trình tái nạp glycogen.

---

## Module K12: Thời điểm Nạp Dinh dưỡng & Động học Hồi phục Chuyển hóa (KN-NTF-01)

### 12.1 Thời điểm Bữa ăn (Nutrient Timing) & "Cửa sổ Anabolic Window"
- **Giải mã Ranh giới Khoa học về Cửa sổ Đồng hóa:**
  - Bằng chứng lịch sử từng tuyên bố có một "cửa sổ 30 phút sau tập" sống còn để uống whey protein ngay lập tức nếu không muốn bị teo cơ.
  - **Khoa học hiện đại xác lập:** Cửa sổ đồng hóa là một **khoảng thời gian rộng từ 4 đến 6 giờ** bao quanh buổi tập (tùy thuộc vào thời điểm và quy mô của bữa ăn trước tập).
  - Nếu đã có bữa ăn chứa protein và carbohydrate đầy đủ cách buổi tập $1-2$ giờ, nồng độ acid amin và glucose trong máu vẫn tiếp tục duy trì mức cao trong suốt buổi tập và kéo dài sang giai đoạn phục hồi. Do đó, việc nạp đạm sau tập là quan trọng, nhưng không mang tính chất khẩn cấp từng phút.
- **Tần suất Nạp Protein trong Ngày:**
  - Chia tổng lượng protein trong ngày thành **$3 - 6$ bữa ăn**, mỗi bữa cách nhau khoảng **$3 - 5$ giờ**, mỗi bữa cung cấp tối thiểu $\ge 0.40 - 0.55\text{ g/kg}$ protein chất lượng cao là cấu trúc tối ưu nhất để kích hoạt lặp lại nhiều lần đỉnh MPS trong 24 giờ mà không gặp phải hiện tượng trơ thụ thể.

### 12.2 Động học Tạm nghỉ Ăn kiêng (Diet Breaks) & Bữa Tái nạp Năng lượng (Refeeds)
- **Refeeds (Nạp lại Năng lượng Ngắn hạn: 1–2 ngày):**
  - Tăng calo trở lại mức duy trì (Maintenance), chủ yếu thông qua việc tăng mạnh carbohydrate trong khi giữ nguyên protein và giữ chất béo ở mức thấp.
  - *Mục tiêu:* Nạp đầy một phần glycogen cơ bắp, hỗ trợ hiệu suất tập luyện cho các buổi tập nặng tiếp theo, kích thích tăng tạm thời hormone Leptin và tạo sự giải tỏa tâm lý ngắn hạn.
- **Diet Breaks (Tạm dừng Ăn kiêng Có chu kỳ: 1–2 tuần liên tục):**
  - Đưa calo về mức duy trì liên tục trong $7 - 14$ ngày sau mỗi chu kỳ siết cân $6 - 12$ tuần.
  - *Cơ chế:* Hạ mức tích tụ mệt mỏi ăn kiêng (diet fatigue), phục hồi một phần nhịp chuyển hóa cơ bản và các hormone tuyến giáp/sinh dục, giảm thiểu tối đa hiện tượng dị hóa khối nạc và cải thiện mạnh mẽ sự gắn bó lâu dài với mục tiêu giảm cân.

---

## Module K13: Phân tầng Bằng chứng & Động học Thực phẩm Bổ sung (KN-SUP-01, KN-SUP-02)

### 13.1 Thang Phân tầng Bằng chứng Thực phẩm Bổ sung
- **Nhóm A (Bằng chứng Vững chắc & Hiệu quả Thực tiễn Rõ rệt):**
  1. *Creatine Monohydrate:* Tăng nồng độ phosphocreatine nội bào $\rightarrow$ tăng tốc độ tái tạo ATP trong các hoạt động bùng nổ $\le 10$ giây $\rightarrow$ tăng trực tiếp sức mạnh, số reps thực hiện và thể tích tế bào (cell swelling). Liều tối thiểu hiệu quả: $3 - 5\text{ g/ngày}$, nạp tích lũy lâu dài, không cần chu kỳ xả nạp.
  2. *Caffeine:* Đối kháng thụ thể Adenosine tại hệ thần kinh trung ương $\rightarrow$ giảm nhận thức về sự gắng sức (RPE), tăng tỉnh táo và tăng khả năng phát lực. Liều dùng hiệu quả: $3 - 6\text{ mg/kg}$ sử dụng trước buổi tập $30-60$ phút.
  3. *Protein Bổ sung (Whey / Casein / Plant isolates):* Đóng vai trò như một nguồn thực phẩm tiện lợi giúp đạt được mục tiêu tổng đạm hàng ngày; không có cơ chế thần thánh vượt trội hơn protein từ thịt cá trứng sữa hoàn chỉnh.
- **Nhóm B (Bằng chứng Hỗn hợp / Lợi ích Biên Có điều kiện):**
  - *Beta-Alanine:* Tăng nồng độ carnosine nội bào $\rightarrow$ đệm ion $H^+$ trong tế bào cơ. Chỉ phát huy tác dụng rõ rệt trong các nỗ lực cường độ cao liên tục kéo dài từ $60$ đến $240$ giây; lợi ích đối với các hiệp tập kháng lực thông thường ($<30-40$ giây) là rất hạn chế.
  - *Citrulline Malate ($6-8\text{ g}$):* Tiền chất tổng hợp Nitric Oxide (NO) $\rightarrow$ giãn mạch, tăng lưu lượng máu và có thể hỗ trợ thanh thải chất chuyển hóa; hiệu quả tăng phì đại trực tiếp còn nhiều tranh cãi.
- **Nhóm C (Bằng chứng Kém / Vô giá trị / Lãng phí Tiền bạc):**
  - *BCAA (khi tổng đạm đã đủ):* Hoàn toàn không mang lại thêm bất kỳ lợi ích nào nếu khẩu phần ăn đã đạt ngưỡng $\ge 1.6\text{ g/kg}$ protein/ngày. BCAA thiếu 6 acid amin thiết yếu còn lại để hoàn tất chu trình MPS.
  - *Fat Burners / Thuốc đốt mỡ:* Chứa các chất kích thích liều cao gây áp lực tim mạch; tác động tiêu hao calo thực tế là không đáng kể so với việc kiểm soát chế độ ăn.
  - *Testosterone Boosters thảo dược:* Không làm tăng nồng độ testosterone vượt qua ngưỡng sinh lý để tạo ra bất kỳ sự phì đại cơ bắp nào ở người có sức khỏe bình thường.

---

## Module K14: Sinh lý Giai đoạn Đỉnh cao & Ranh giới Nguy cơ Cắt cân (KN-CPW-01, KN-CPW-02)

### 14.1 Sinh lý Học Giai đoạn Đỉnh (Physique Peaking Mechanics)
- **Siêu bù Glycogen (Glycogen Supercompensation / Carb Loading):**
  - Tận dụng trạng thái cạn kiệt glycogen trước đó để nạp lượng lớn carbohydrate ($8 - 12\text{ g/kg}$ carb) trong $24 - 48$ giờ trước khi lên sàn.
  - Glycogen tích lũy tối đa trong sợi cơ kéo theo nước từ khoang gian bào vào trong sợi cơ $\rightarrow$ tạo diện mạo bắp cơ căng tròn tối đa và làm mỏng lớp mô dưới da.
- **Khoang Nước Thể dịch (Water Compartmentalization):**
  - Nước trong cơ thể phân bố ở hai khu vực chính: Nội bào (Intracellular Fluid - ICF, chiếm $\sim 65-70\%$) và Ngoại bào (Extracellular Fluid - ECF, bao gồm huyết tương và nước dưới da gian bào).
  - Mục tiêu tối thượng của physique peaking là tối đa hóa ICF (cơ căng đầy) trong khi tối thiểu hóa ECF gian bào (da mỏng bám sát cơ).

### 14.2 Ranh giới An toàn Nghiêm ngặt về Cắt cân Cấp tính (Weight-Making Risks)
- **Cơ chế Cắt nước Cưỡng bức (Water Manipulation & Dehydration Hazards):**
  - Việc cắt giảm đột ngột nước uống kết hợp xông hơi (sauna) hoặc dùng thuốc lợi tiểu (diuretics) làm sụt giảm nghiêm trọng thể tích máu lưu hành (hypovolemia).
  - *Nguy cơ Chết người:* Rối loạn điện giải cấp tính ($Na^+$, $K^+$ bất thường) dẫn đến chuột rút toàn thân, tụt huyết áp tư thế, suy thận cấp, rối loạn nhịp tim và đột quỵ do trụy tim mạch.
- **Quy tắc An toàn Tuyệt đối của Hệ thống:**
  - HỆ THỐNG TUYỆT ĐỐI KHÔNG CUNG CẤP PHÁC ĐỒ CẮT NƯỚC, CẮT MUỐI CẤP TÍNH HOẶC SỬ DỤNG LỢI TIỂU CHO BẤT KỲ MỤC ĐÍCH NÀO (Kích hoạt ngay ngắt an toàn `TRG-13` / `SC-C` / `OA-11`).

---

## Module K15: Phục hồi Nội tiết Sau Thi đấu & Chu kỳ hóa Dinh dưỡng (KN-PCR-01, KN-PCR-02)

### 15.1 Khủng hoảng Sinh lý Sau Thi đấu & Trục Nội tiết Bị Ức chế
- Vận động viên thể hình ở giai đoạn thi đấu (tỷ lệ mỡ cực thấp: $\sim 4-6\%$ ở nam, $\sim 10-12\%$ ở nữ) rơi vào trạng thái khủng hoảng sinh học sâu sắc:
  - Trục Dưới đồi - Tuyến yên - Tuyến sinh dục (HPG axis) bị ức chế hoàn toàn: Nồng độ testosterone ở nam rơi xuống mức thiến bệnh lý; nữ giới mất kinh nguyệt hoàn toàn.
  - Tỷ lệ trao đổi chất suy giảm cực đại, hệ miễn dịch suy yếu, mất ngủ trầm cảm và cảm giác thèm ăn vô độ (hyperphagia).
- **Hội chứng Ăn uống Mất kiểm soát (Post-Show Bingeing):**
  - Việc ăn thả cửa không kiểm soát ngay sau cuộc thi dẫn đến tích nước phù nề cấp tính, tăng mỡ ồ ạt trong khi các tế bào mỡ mới có thể được sản sinh (adipocyte hyperplasia), để lại hậu quả chuyển hóa tiêu cực lâu dài.

### 15.2 Động học Hồi phục Dinh dưỡng (Recovery Diet vs. Reverse Dieting)
- **Reverse Dieting (Tăng Calo Siêu chậm):**
  - Tăng từng $50 - 100\text{ kcal}$ mỗi tuần.
  - *Nhược điểm Sinh lý:* Kéo dài thời gian cơ thể phải chịu đựng trạng thái thiếu hụt năng lượng khả dụng (LEA); trục nội tiết tiếp tục bị đình trệ thêm nhiều tháng.
- **Recovery Diet (Phương pháp Hồi phục Nhanh có Kiểm soát):**
  - Ngay lập tức đưa mức calo trở lại mức Duy trì Mới hoặc thặng dư nhẹ ($+200 - 400\text{ kcal}$), chấp nhận tăng nhanh một lượng mỡ lành mạnh nhất định ($3 - 5\text{ kg}$) trong $2 - 4$ tuần đầu để tái lập mức mỡ tối thiểu bảo đảm sự hồi phục của Leptin, hormone tuyến giáp và hormone sinh dục.

### 15.3 Chu kỳ hóa Dinh dưỡng Dài hạn (Macrocycle Nutrition Periodization)
- Tổ chức các giai đoạn dinh dưỡng đồng bộ với chu kỳ tập luyện trong năm:
  $$\text{Hypertrophy Phase (Surplus nhẹ)} \longrightarrow \text{Consolidation / Maintenance} \longrightarrow \text{Fat Loss / Cut} \longrightarrow \text{Post-Cut Restabilization}$$
- Không duy trì trạng thái siết cân cắt calo liên tục quá $12-16$ tuần mà không có giai đoạn tái lập chuyển hóa ở mức duy trì.

---

## Module K16: Tâm lý học Hành vi Ăn kiêng & Thần kinh Thể dịch Lối sống (KN-NBA-01, KN-NBA-02)

### 16.1 Bản thể học Kiểm soát Nhận thức (Cognitive Restraint)
- **Kiểm soát Cứng nhắc (Rigid Restraint / All-or-Nothing Mentality):**
  - Phân loại thực phẩm thành hai thái cực tuyệt đối: "Đồ sạch" (Clean) vs "Đồ bẩn/Tội lỗi" (Dirty/Cheat).
  - *Cơ chế Thất bại:* Khi lỡ ăn một lượng nhỏ đồ ăn "bị cấm", người ăn kiêng kích hoạt hiện tượng "Hiệu ứng Đằng nào cũng lỡ" (What-the-hell Effect) $\rightarrow$ mất kiểm soát hoàn toàn và ăn vô độ, tiếp nối bằng cảm giác tội lỗi và trừng phạt bản thân bằng cách nhịn ăn hoặc tập cardio cưỡng bức.
- **Kiểm soát Linh hoạt (Flexible Dieting / IIFYM):**
  - Tiếp cận dinh dưỡng dựa trên mục tiêu năng lượng và đại dưỡng chất tổng quát.
  - Phân bổ thực phẩm theo quy tắc **$80/20$**: Tối thiểu $80\%$ năng lượng đến từ các thực phẩm toàn phần giàu vi chất và chất xơ; dành tối đa $20\%$ linh hoạt cho các sở thích ăn uống cá nhân để duy trì sự thỏa mãn tâm lý và hòa nhập xã hội.

### 16.2 Bản thể học Mức độ Chính xác Theo dõi (Tracking Tiers)
- Không bắt buộc mọi cá nhân đều phải cân đo từng gram thức ăn suốt đời:
  - *Tier 1 (Habit-based / Qualitative):* Dựa trên kích thước nắm tay, đĩa thức ăn, ăn chậm nhai kỹ và lắng nghe tín hiệu no/đói. Phù hợp cho người mới bắt đầu hoặc mục tiêu sức khỏe tổng quát.
  - *Tier 2 (Calorie & Protein Tracking):* Chỉ theo dõi tổng năng lượng và lượng đạm, linh hoạt carb/fat. Phù hợp cho đa số mục tiêu thể hình thực tế.
  - *Tier 3 (Precise Macro Tracking):* Cân đo chính xác toàn bộ calo và từng gram macro. Chỉ cần thiết cho giai đoạn siết cân sâu tiệm cận thi đấu.

### 16.3 Trục Giao tiếp Thần kinh Thể dịch: Giấc ngủ, Stress & Chuyển hóa
- **Mất ngủ Mãn tính ($<7$ giờ/đêm):**
  - Tăng nồng độ **Ghrelin** (hormone gây cảm giác đói) và giảm nồng độ **Leptin** (hormone báo no) $\rightarrow$ kích thích sự thèm ăn đặc biệt đối với các thực phẩm giàu đường và chất béo bão hòa.
  - Suy giảm độ nhạy insulin ngoại vi lên đến $30\%$, tương đương trạng thái tiền tiểu đường tạm thời.
  - Thay đổi P-ratio bất lợi: Trong cùng một mức thâm hụt calo, người thiếu ngủ bị mất tỷ lệ mô nạc nhiều hơn và mất ít mỡ hơn so với người ngủ đủ giấc.
- **Căng thẳng Tâm lý & Nồng độ Cortisol Kéo dài:**
  - Cortisol tăng mãn tính thúc đẩy quá trình dị hóa protein cơ bắp, tăng tích lũy mỡ nội tạng (visceral fat) và gây giữ nước dưới da gian bào $\rightarrow$ che mờ tiến độ giảm mỡ thực tế trên cân và thước đo.

---

# MẠNG LƯỚI QUAN HỆ NHÂN QUẢ LIÊN MODULE (CROSS-MODULE CAUSAL GRAPH)

```text
                                  [KINH NGHIỆM / CƠ ĐỊA / TUỔI / GIỚI] (K07)
                                                     │
                                                     ▼
[CÂN BẰNG NĂNG LƯỢNG (K09)] ───────► [KHỐI LƯỢNG TẬP LUYỆN (K04)] ──────► [SỨC CĂNG CƠ HỌC (K02)]
           │                                         │                                 │
           ▼                                         ▼                                 ▼
[ĐẠI DƯỠNG CHẤT (K10)] ──────────────► [KHẢ NĂNG PHỤC HỒI / MRV (K08)] ──► [PHÌ ĐẠI CƠ BẮP (K01)]
           │                                         ▲
           ▼                                         │
[GIẤC NGỦ / LỐI SỐNG (K16)] ─────────────────────────┘
```

---
*End of fitness-theory-ontology.md — Quad-File Production Knowledge Layer (File 2/4)*

