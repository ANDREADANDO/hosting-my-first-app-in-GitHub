import streamlit as st

st.title("Calculator")

num1 = st.number_input("Enter first number", value=0.0)
num2 = st.number_input("Enter second number", value=0.0)

st.write("Choose an operation:")
operation = st.selectbox(
    "Operation",
    ("Add", "Subtract", "Multiply", "Divide")
)

if st.button("Calculate"):
    if operation == "Add":
        result = num1 + num2
        st.success(f"Result: {result}")

    elif operation == "Subtract":
        result = num1 - num2
        st.success(f"Result: {result}")

    elif operation == "Multiply":
        result = num1 * num2
        st.success(f"Result: {result}")

    elif operation == "Divide":
        if num2 != 0:
            result = num1 / num2
            st.success(f"Result: {result}")
        else:
            st.error("Error: Cannot divide by zero")
