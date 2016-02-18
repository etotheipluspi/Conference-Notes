Balanchandran, Atkins

Ella Atkins talk at Stanford

Filgt safety assesment as MDP:
    * What state feautes are needed to model loss of control
        - Assume full state observability (Should use a POMDP)
        - Aircraft dynamics
        - Complete state space is huge: position, vel, status of spoliers, rudders, etc
            - Aircraft state vector
            - Status of onbaord controllers
            - Aircraft health
            - Flight crew characteristic
            - Environment chracteristics
            - 30-40 variables ... (huge space)
    * Action space:
        - Cockpit control inputs + no actions
    * Reward:
        - Penalized for unsafe states (speed, altitude, etc)

Approach:
    * Sampling based (to some horizon) expectation approach to Bellmand updated
    * Use generative to sample state space
    * Assume environemnt variables reamin constant, fligh crew constant, health constant (why health constant when doing safety assesment?)

