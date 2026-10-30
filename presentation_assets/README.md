# Conference Presentation Asset Package & Verified CSV Data

This folder contains high-resolution (300 DPI, $\ge 2000\text{ px}$ width) publication-grade plots and raw data CSVs generated strictly from the project's frozen zero-leakage benchmark (`dataset_v1_frozen`).

Repository: [givemehat/ONLINETIHIITG](https://github.com/givemehat/ONLINETIHIITG)  
Assets Directory: [presentation_assets](https://github.com/givemehat/ONLINETIHIITG/tree/main/presentation_assets)  
Raw CSV Data Directory: [presentation_assets/csv_data](https://github.com/givemehat/ONLINETIHIITG/tree/main/presentation_assets/csv_data)

---

## 1. Top 5 Priority Presentation Figures (Requested by User)

| Priority & Slide | Plot Filename & Description | Corresponding Raw CSV Data | Direct GitHub Link |
| :--- | :--- | :--- | :--- |
| **#1. Slide 11 (Results)** | `Plot1_Slide11_Predicted_vs_Actual_SOH_600_windows.png`<br>3-panel predicted vs. actual SOH parity plot (LSTM, GRU, TCN) across all 600 operational test windows with 45° line & $\pm 5\%$ envelope. | `csv_data/soh_predictions_600_test_windows.csv` | [View Plot 1](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot1_Slide11_Predicted_vs_Actual_SOH_600_windows.png) |
| **#1A. Slide 11 (Master Dual)** | `Slide11_Dual_Scenario_Master_Explanation.png`<br>**Master Infographic**: 2 Histograms showing the B0036 Variance Trap + 2 Parity plots + Complete 5-model benchmark table side-by-side. | `csv_data/dual_case_model_comparison_table.csv` | [View Master Dual Chart](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide11_Dual_Scenario_Master_Explanation.png) |
| **#1B. Slide 11 (Dual Table)** | `Slide11_Dual_Case_Accuracy_Table.png`<br>Side-by-side comparison table comparing Case 1 (Raw Fleet $R^2=0.814$) vs Case 2 (Full Lifecycle $R^2=0.924$) with invariant MAE ~2.5%. | `csv_data/dual_case_model_comparison_table.csv` | [View Dual Table](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide11_Dual_Case_Accuracy_Table.png) |
| **#1C. Slide 11 (Dual Parity)** | `Slide11_Dual_Case_SOH_Parity_Comparison.png`<br>Dual-case side-by-side parity scatter highlighting the B0036 cluster in Case 1 vs. uniform dynamic spread in Case 2. | `csv_data/soh_predictions_600_test_windows.csv` | [View Dual Parity](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide11_Dual_Case_SOH_Parity_Comparison.png) |
| **#1D. Slide 11 (Math Proof)** | `Slide11_Why_R2_Differs_Variance_Explanation.png`<br>Visual formula diagram explaining $R^2 = 1 - \frac{\text{MSE}}{\text{Var}(y)}$ and why MAE is the invariant engineering metric. | — | [View Math Proof](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide11_Why_R2_Differs_Variance_Explanation.png) |
| **#2. Slide 12 (Robustness)**| `Plot2_Slide12_Per_Cell_Robustness_Bar_Chart.png`<br>Grouped bar chart showing SOH MAE and $R^2$ across all 9 holdout test cells (proves cross-cell transfer without identity leakage). | `csv_data/per_cell_test_metrics.csv` | [View Plot 2](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot2_Slide12_Per_Cell_Robustness_Bar_Chart.png) |
| **#3. Slide 12 (Stages)** | `Plot3_Slide12_Stage_Wise_MAE_Robustness.png`<br>Degradation stage MAE comparison across Healthy ($>85\%$), Knee Transition ($70-85\%$), and Accelerated Aging ($<70\%$). | `csv_data/stage_wise_mae_metrics.csv` | [View Plot 3](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot3_Slide12_Stage_Wise_MAE_Robustness.png) |
| **#4. Slide 12/14 (RUL)** | `Plot4_Slide12_B0018_RUL_Predictions_Clean.png`<br>Clean cycle countdown on test cell B0018 showing **strictly Ridge, RF, LSTM, GRU, and TCN** against actual ground truth (no unverified models). | `csv_data/b0018_rul_predictions.csv` | [View Plot 4](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot4_Slide12_B0018_RUL_Predictions_Clean.png) |
| **#5. Slide 07 (Pipeline)** | `Plot5_Slide07_Early_500s_Discharge_Curves.png`<br>3-panel synchronized physical telemetry over the first 500s ($t \in [0, 500\text{ s}]$, 51 steps): Terminal Voltage Sag, 2.0A CC Current, Thermal Rise $\Delta T$. | `csv_data/discharge_early_500s_telemetry.csv` | [View Plot 5](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot5_Slide07_Early_500s_Discharge_Curves.png) |

---

## 2. Additional Essential Assets

| Topic & Slide | Asset Filename & Description | Direct GitHub Link |
| :--- | :--- | :--- |
| **Real Training Loss** | `Plot6_Real_Logged_Training_Validation_Loss.png`<br>Real epoch-by-epoch MSE training and validation loss curves logged directly during model training (no spikes). CSV: `csv_data/real_training_loss_curves.csv`. | [View Loss Plot](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot6_Real_Logged_Training_Validation_Loss.png) |
| **AUV Schematic (Slide 2)** | `Plot7_AUV_Subsea_System_Schematic.png`<br>Clean vector schematic of an Autonomous Underwater Vehicle with onboard battery pack, acoustic sonar, propulsion thrusters, and edge BMS engine. | [View AUV Vector](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Plot7_AUV_Subsea_System_Schematic.png) |
| **Knee Transition Anatomy** | `Slide03B_Knee_Transition_Point_Anatomy.png`<br>Geometric two-tangent asymptote intersection defining the knee point (Cycle ≈ 68 on B0006) + cross-cell knee variability. | [View Knee Chart](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide03B_Knee_Transition_Point_Anatomy.png) |
| **Why No BiLSTM (Slide 9)** | `Slide09_Why_No_BiLSTM_Causality_Violation.png`<br>Causal timeline diagram showing why backward RNN passes require unobserved future data and violate online BMS causality. | [View Causality Diagram](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide09_Why_No_BiLSTM_Causality_Violation.png) |
| **Fleet Capacity Fade (Slide 12)**| `Slide12_NASA_Fleet_Capacity_Fade_By_Temperature.png`<br>Comprehensive 6-panel chart of all 34 NASA cells across 4°C, 22°C, 24°C, 43°C, 44°C with master legend. | [View Fleet Plot](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide12_NASA_Fleet_Capacity_Fade_By_Temperature.png) |
| **SOH Trajectories (Slide 13)** | `Slide13_SOH_Degradation_Trajectories.png`<br>Full fleet SOH fade curves with 85% healthy, 80% knee warning, and 70% EOL boundaries. | [View Trajectories](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide13_SOH_Degradation_Trajectories.png) |
| **Signal Decomposition (Slide 15)**| `Slide15_Signal_Decomposition_Recovery_vs_Trend.png`<br>Decoupling irreversible thermodynamic fade from reversible rest-recovery shocks. | [View Decomposition](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide15_Signal_Decomposition_Recovery_vs_Trend.png) |
| **Baseline Parity Scatter (Slide 19)**| `Slide19_Baseline_ML_Parity_Scatter.png`<br>High scatter and failure of Ridge ($R^2 = -3.74$) and Random Forest ($R^2 = -3.48$, RUL MAE $\approx 107$). | [View Baseline Scatter](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide19_Baseline_ML_Parity_Scatter.png) |
| **Data Provenance Fix (Slide 18)**| `Slide18_Data_Provenance_Fix_Before_After.png`<br>The $-24.40$ to $+0.883$ root cause fix: corrupted $0.05\text{ Ah}$ discharges vs. cleaned multi-cycle formation baseline. | [View Provenance Fix](https://github.com/givemehat/ONLINETIHIITG/blob/main/presentation_assets/Slide18_Data_Provenance_Fix_Before_After.png) |
