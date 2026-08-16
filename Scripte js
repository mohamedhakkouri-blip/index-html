const display = document.getElementById("display");

function appendValue(value) {
    if (display.value === "0") {
        display.value = value;
    } else {
        display.value += value;
    }
}

function clearDisplay() {
    display.value = "0";
}

function deleteChar() {
    if (display.value.length > 1) {
        display.value = display.value.slice(0, -1);
    } else {
        display.value = "0";
    }
}

function calculate() {
    try {
        const result = eval(display.value);

        if (!isFinite(result)) {
            display.value = "Erreur";
        } else {
            display.value = result;
        }
    } catch (error) {
        display.value = "Erreur";
    }
}
