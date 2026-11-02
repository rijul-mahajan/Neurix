# Neurix

**Explore how neural networks process information — and learn how they learn.**

Neurix is an interactive, browser-based playground for understanding neural networks. Visualize signals moving through layers of neurons, inspect weights and activations, and train a small network on familiar logic gates using gradient descent and backpropagation.

**[Launch Neurix](https://rijul-mahajan.github.io/Neurix/)**

---

## What you can do

### Explore mode

Watch a neural network perform forward propagation in real time.

- Configure a network with **2–6 layers** and **2–12 neurons per hidden layer**.
- Choose hidden-layer activation functions: **Sigmoid, Tanh, ReLU,** or **Leaky ReLU**.
- Choose an output activation: **Sigmoid** or **Softmax**.
- Switch between automatic input signals and manual input values.
- Generate new weights or reset the network settings.
- Customize node and edge colors, glow intensity, edge coloring, and activation-value labels.

Select any neuron to inspect its activation and the weighted-sum calculation that produced it. Hover over a connection to examine its weight and the signal it carries.

### Train mode

Experiment with a small neural network learning Boolean logic.

- Train on **XOR, AND, OR,** and **XNOR** datasets.
- Adjust the learning rate.
- Watch the network update its weights through backpropagation and gradient descent.
- Follow training progress through the loss and accuracy statistics.
- View the decision-boundary plot as the network learns.

The visualizer also illustrates why a network without a hidden layer cannot learn XOR, and how adding a hidden layer makes that task possible.

---

## Controls

| Control | Action |
|---|---|
| Play / Pause | Start or pause the animation or training |
| Step | Advance the simulation; in Train mode, perform a short training step |
| Restart | Restart using the same initial weights |
| New weights | Generate a new set of network weights |
| Reset settings | Restore the default configuration |
| Theme toggle | Switch between dark and light themes |

### Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Space` | Play or pause |
| `N` | Step |
| `R` | Restart |

---

## Run locally

No build tools, package managers, dependencies, or backend are required.

1. Clone the repository:

   ```bash
   git clone https://github.com/rijul-mahajan/Neurix.git
   cd Neurix
   ```

2. Open `index.html` in a modern browser.

You can also serve the folder locally:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

---

## Built with

- HTML
- CSS
- JavaScript
- HTML Canvas for network rendering and training charts

The application runs entirely in the browser. Inter and JetBrains Mono are loaded from Google Fonts, with system font fallbacks available.

## Contributing

Ideas, bug reports, and improvements are welcome. Open an issue to report a problem or suggest a new feature. Pull requests are welcome.
