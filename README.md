# ColdAtom-Quantum-Simulator v3.0
A browser-based **verifiable cold atom lattice simulator** for computational physics research and education, implemented with HTML5 + Canvas + JavaScript. No environment configuration required — open in any browser and use immediately.

This simulator realizes **physical coupling, observable calculation and falsifiable experimental design** based on the deep lattice approximation of cold atom physics, and supports real-time adjustment of key parameters, superfluid-insulator phase transition exploration, and theoretical/experimental mode comparison.

## 🌟 Core Features
1. **Physical Coupling (V₀ → t)**  
   The hopping integral `t` is dynamically calculated by the lattice depth `V₀` (based on the deep lattice approximation formula), and the effective `U/t` is updated in real time to ensure physical self-consistency.
2. **Key Observable Calculation**  
   Real-time display of superfluid order parameter `|⟨a⟩|`, number fluctuation `Δn`, and momentum distribution (TOF simulation, structure factor S(k) calculation).
3. **Falsifiable Experimental Mode**  
   - **Experimental Mode**: Blank phase diagram, click to record "experimental results" and explore the phase transition boundary by yourself.
   - **Theoretical Mode**: Pre-computed full phase diagram with a white dashed line for the theoretical critical boundary (U_c/t ≈ 25).
   - Support resetting exploration records for repeated verification.
4. **Lightweight & Interactive**  
   8×8 real-space lattice visualization, mouse hover probe, one-click mode switching, and real-time update of all physical results with parameter adjustment.

## 🚀 Quick Start
### 1. Run Directly
- Download the core file `ColdAtom_Simulator_v3.0.html` from the repository.
- Double-click the file to open it in **any browser** (Chrome/Edge/Firefox/Safari).
- No installation, no dependencies, no GPU/CPU requirements.

### 2. Basic Operation
- **Adjust Parameters**: Slide to change lattice depth `V₀` and interaction `U`, all physical results update in real time.
- **Lattice Probe**: Hover the mouse over the 8×8 lattice to view the local density of the lattice site.
- **Phase Diagram Exploration**: Click the phase diagram to jump to the corresponding parameters and record experimental points (Experimental Mode).
- **Mode Switch**: Toggle between "Experimental Mode" and "Theoretical Mode" to compare with the theoretical phase boundary.
- **TOF Visualization**: The momentum distribution panel shows the coherence peak (superfluid phase) or diffuse distribution (insulator phase) in real time.

## 📚 Physical Background
Based on the cold atom optical lattice system, the core physical models include:
- Hopping integral: `t ≈ (4/√π) * V₀^(3/4) * exp(-2√V₀)` (Deep lattice approximation, Er=1)
- Superfluid order parameter: `|⟨a⟩| = ⟨√n⟩` (Mean-field approximation)
- Number fluctuation: `Δn = √(⟨n²⟩ - ⟨n⟩²)`
- Momentum distribution: Structure factor `S(k) = |∑ e^(ikr) n_r|²` (TOF simulation)
- Superfluid-insulator transition critical boundary: `U_c/t ≈ 25` (Unit filling)

## 🛠️ Technical Stack
- Frontend: HTML5 + Canvas (visualization) + Vanilla JavaScript (physical calculation & interaction)
- Dependence: Only `numeric.min.js` (for matrix eigenvalue calculation, CDN introduced)
- Compatibility: Support all modern browsers (PC/macOS/Pad), responsive layout.

## 📖 Use Cases
1. **Computational Physics Research**: Pre-research of cold atom lattice experiment parameters, quick screening of V₀/U/t effective range, and phase transition trend verification.
2. **University Education**: Teaching tool for *Cold Atom Physics*, *Condensed Matter Physics* and *Quantum Simulation* (undergraduate/graduate level), making abstract physical concepts intuitive.
3. **Science Popularization**: Popular science demonstration of quantum phase transition for scientific research institutions and science and technology museums.

## 📌 Version Update
- **v3.0 (Latest)**: Realize physical coupling, observable calculation and falsifiable experimental mode (core upgrade).
- **v2.0**: Basic lattice visualization and parameter adjustment (visual demo version).
- **v1.0**: Prototype of cold atom lattice density simulation.

## 🧑💻 Author
Independent researcher focusing on the intersection of **AI for Science** and **computational atomic physics**.

## 📄 License
This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details. Free for commercial/non-commercial use, modification and distribution, with only the copyright statement retained.

---

### 中文版本（冷原子量子模拟器 v3.0）
本项目是一款基于HTML5的**浏览器端可验证冷原子晶格物理模拟器**，无需配置环境，打开即用，适用于计算物理科研预研和高校教学。

模拟器基于冷原子物理深晶格近似，实现了**物理耦合、可观测量计算、可证伪实验设计**三大核心功能，支持关键参数实时调节、超流-绝缘相变探索、理论/实验模式对比。

#### 核心功能（中文）
1. **物理耦合**：晶格深度V₀动态决定跃迁积分t，有效U/t实时更新，保证物理自洽；
2. **可观测量计算**：实时显示超流序参量|⟨a⟩|、数涨落Δn、动量分布（TOF飞行时间模拟）；
3. **可证伪实验模式**：实验模式（空白相图，点击记录实验点）、理论模式（预计算全相图+理论临界边界），支持重置探索；
4. **轻量交互**：8×8实空间晶格可视化、鼠标悬停探针、参数调节实时刷新所有物理结果。

#### 快速开始（中文）
1. 从仓库下载核心文件`ColdAtom_Simulator_v3.0.html`；
2. 双击文件，用任意浏览器打开即可使用，无安装、无依赖；
3. 滑动调节V₀（晶格深度）、U（相互作用），点击相图探索相变，切换模式对比理论边界。

#### 物理背景（中文）
基于冷原子光晶格系统，核心模型包含跃迁积分深晶格近似、超流序参量平均场近似、结构因子动量分布计算，超流-绝缘相变理论临界边界U_c/t≈25（单位填充）。

#### 许可证
本项目采用**MIT开源协议**，可免费用于商业/非商业用途、修改和分发，仅需保留版权声明。
