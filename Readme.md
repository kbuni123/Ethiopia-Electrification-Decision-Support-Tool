# Header
    st.title("⚡ Ethiopia Electrification Decision Support Tool")
    with st.expander("ℹ️ About this Tool – Click to Expand"):
        st.markdown(
            """
            ### Complete Electrification Analysis
            This tool is an **energy modeling and decision-support platform** built to explore Ethiopia’s 
            pathways to achieving **100% electrification by 2030**. It combines the World Bank's DRE-ATLAS data, user defined technology 
            cost models, and financing scenarios into an interactive Streamlit application that allows 
            policymakers, planners, and researchers to test different electrification strategies.

            ---
            #### ⚙️ How it Works

            **Pre-Step – Electrification Status Check**  
            - Uses satellite nightlight data from the DRE atlas to identify which settlements are already electrified.  
            - Separates settlements into *electrified* and *unelectrified*.  

            **Step 1 – Full Electrification Cost Calculation**  
            - Calculates the **total cost** of providing electricity to all unelectrified settlements without budget constraints. The cost of the technology is defined by the user.
            - The technology for a settlement is selected based on settlement characteristics(road access, distance from existing grid, population size).
            
            **Step 2 – Budget-Constrained Optimization with**  
            - Uses the Step 1 total cost as the baseline.  
            - Lets the user distribute the total cost as **percentages across 2025–2030** to simulate phased electrification.  
            - Lets the user to adjust weights to balance competing objectives for prioritizing the electrification of a settlement.
            - Generates maps and tables showing rollout progress, budget use, and technology mix.  
            """
        )
