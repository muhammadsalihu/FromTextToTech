All software provided here is distributed freely under the Creative Commons Attribution-NonCommercial-ShareAlike (CC BY-NC-SA) license. This license allows for sharing, adapting, and building upon the material non-commercially, as long as appropriate credit is given and any new creations are licensed under identical terms.

These notebooks serve as supplementary material for the manuscript 'From Text to Tech: Shaping the Future of Physics-Based Simulations with AI-Driven Generative Models' by Alessio Alexiadis and Bahman Ghiassi. They were instrumental in generating the test cases 'square_bar' and 'wheel_axle', with each test case organized into '.\geometry' and '.\simulation' files.

Please note that the software is provided 'as is' without any warranties or guarantees of performance or reliability. Additionally, an OpenAI key is required to run the test cases, which is not provided with the software.

USAGE
In the notebooks, the GPT-4 1106-preview model is utilized through the OpenAI API within the chat_with_bot() function. To guide the LLM in generating outputs, we use two prompt files: system_geo.txt for geometry creation and system_sif.txt for simulation parameters and conditions. These prompt files are also included in the supplementary materials. 
The LLM's output is then processed through the extract_and_save_geo_file() and extract_and_save_sif_file() functions. The workflow is completed by interacting with the Gmsh's API for meshing and by executing external system commands within the Python environment, specifically !ElmerGrid and !ElmerSolver, to process the mesh and run the simulations
