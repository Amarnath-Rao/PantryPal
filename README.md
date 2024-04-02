# PantryPal

![_2965934b-a70c-4dca-b4e6-f428ffdd3b2a](https://github.com/Amarnath-Rao/PantryPal/assets/96937608/1a91da40-5313-424e-8686-223dabe704af)


PantryPal is an MVP application that suggests recipes based on the contents of your fridge. Users can upload photos of their fridge, set some parameters, and receive suggestions on what to cook along with the steps based on their parameters and items.

### Project Structure

- `main.py`: This is the main file that contains the Streamlit-powered user interface.
- `models`: This directory contains the Text and Vision models which run the Gemini API.
- `tests`: This directory contains various test files that use TruLens to test different models.

### Project Purpose

PantryPal was developed with the aim of simplifying meal planning and cooking by leveraging AI technology. The project addresses the common challenge of deciding what to cook based on the ingredients available in one's pantry or fridge. By using AI-powered image recognition and natural language processing, PantryPal suggests recipes tailored to the user's available ingredients, dietary preferences, and cooking time constraints. This innovative approach not only promotes efficient use of food resources but also enhances the cooking experience for users by providing personalized recipe recommendations.

### Role of AI

1. **Ingredient Recognition**: AI models are employed to analyze uploaded images of ingredients and identify them accurately. This enables users to effortlessly capture and upload images of their pantry or fridge without the need for manual input.

2. **Recipe Suggestions**: Natural language processing models are utilized to generate recipe suggestions based on the recognized ingredients. By considering factors such as dietary preferences, cooking time, and available ingredients, the AI algorithms provide personalized recipe recommendations to users.

3. **Enhanced User Experience**: The integration of AI technology enhances the user experience by simplifying the meal planning process and offering tailored recommendations. Users can explore a variety of recipe options that align with their preferences and ingredient availability, making cooking more enjoyable and convenient.

4. **Continuous Improvement**: The AI components of PantryPal are designed to learn and adapt over time based on user interactions and feedback. This iterative process allows the system to continuously improve its recommendations and better serve the needs of users.


### Description

Flagsmith can serve as:

1. **Feature Flag Management**: Flagsmith can help manage features within your application. For example, our project use feature flags to toggle certain functionalities or UI elements based on user feedback or experimental data.

2. **Experimentation and A/B Testing**: Flagsmith can facilitate A/B testing by allowing our project to roll out new features or changes to a subset of users. This way, our project can gauge user response and iterate on features before fully deploying them.

3. **Dynamic Configuration**: You can dynamically configure aspects of your application using Flagsmith. For instance, our project adjust the behavior of certain components based on user preferences or external conditions.

4. **Rollout Control**: Flagsmith enables controlled feature rollouts, allowing our project to gradually introduce new features to your user base. This helps mitigate risks associated with large-scale deployments and allows for smoother transitions.

5. **Real-time Updates**: With Flagsmith, our project can make changes to feature flags in real-time without redeploying your application. This flexibility allows for rapid iteration and responsiveness to changing user needs or market conditions.

- Overall, Flagsmith enhances the agility, control, and adaptability of your application by providing a centralized platform for managing feature flags and configurations. It empowers project to make data-driven decisions, experiment with new ideas, and optimize user experiences more effectively.

- Through Flagsmith SaaS, we could have seamlessly deployed our project, PantryPal, by leveraging its feature flag and configuration management capabilities. Flagsmith would have allowed us to control feature rollouts, experiment with new functionalities, and dynamically configure aspects of our application in real-time. By utilizing Flagsmith, we could have enhanced the agility and adaptability of our project, enabling us to make data-driven decisions and optimize user experiences more effectively.

- Due to technical issues with MindsDB, such as syntax errors when creating tables and inserting data, as well as memory limitations when hosting on a server, the project opted to explore alternative solutions. This led to consideration of using Prisma as a reliable data source for saving data.




https://github.com/Amarnath-Rao/PantryPal/assets/96937608/87800682-4661-4e55-9863-a779f0cb95a0



### Setup

1. **Clone the repository:**

    ```
    git clone git@github.com:AmarnathRao/PantryPal.git
    ```

2. **Navigate into the project directory:**

    ```
    cd PantryPal
    ```

3. **Install the required dependencies:**

    ```
    pip install -r requirements.txt
    ```

    Note: It's recommended to use a virtual environment to avoid conflicts with other packages.

4. **Export your Google API key:**

    ```
    export GOOGLE_API_KEY=<your_google_api_key>
    ```

5. **Export your OpenAI API key:**

    ```
    export OPENAI_API_KEY=<your_openai_api_key>
    ```

6. **Export your Flagsmith environment key:**

    ```
    export FLAGSMITH_ENV_KEY=<your_flagsmith_environment_key>
    ```

### Running the Application

1. **Run the Streamlit application:**

    ```
    streamlit run main.py
    ```

2. **Open your web browser and visit [http://localhost:8501](http://localhost:8501) to view the application.**


![image](https://github.com/Amarnath-Rao/PantryPal/assets/96937608/136caa2a-b296-44c5-a34a-8f6ec681bdef)

### Running the Tests

1. **Run the tests:**

    ```
    pytest tests
    ```
