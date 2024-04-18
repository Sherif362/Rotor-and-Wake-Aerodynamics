This project involved developing a Blade Element Momentum (BEM) code in Python to analyze the performance of wind turbines and propellers. The code incorporates essential corrections for heavily loaded rotors (Glauert) and tip/root losses (Prandtl).

Project Scope:

    Airfoil Selection:
        Wind Turbine: DU airfoil (polar provided)
        Propeller: ARA-D 8% airfoil (polar assumed available)
    Wind Turbine Baseline Design:
        Radius: 50 m
        Blade Count: 3
        Blade Start: 0.2 r/R (circular root section ignored)
        Twist Distribution: 14*(1-r/R) (for r/R > 0.2)
        Blade Pitch: -2 degrees
        Chord Distribution: (3*(1-r/R)+1) m (for r/R > 0.2)
        Operational Conditions:
            Wind Speed (U0): 10 m/s
            Tip Speed Ratio (TSR): 6, 8, 10
            Yaw Angle: 0, 15, 30 degrees (optional)
    Analysis Tasks:
        Mandatory: Calculate performance for axial flow cases at varying TSRs.
        Optional: Calculate performance for yawed flow cases (TSR = 8).
        Optional: Optimize design for maximum Cp at TSR = 8 and CT = 0.75 (axial flow) by adjusting pitch, chord, or twist distribution. Compare with actuator disk theory expectations.
