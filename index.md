# Flow [Architectures](https://ukb-dt.github.io/iago/) Across Domains

## The Core Metaphor: Resource Flow → Combinatorial Search → Power/Energy Output

| Level | Tree Biology | Human Exercise Physiology | Neural Network Training |
|-------|-------------|---------------------------|------------------------|
| **Substrate/Soil** | Minerals, water, nutrients in soil | Glucose/glycogen, fatty acids, oxygen in blood | Training data, labeled examples |
| **Distribution Network** | Root system (combinatorial search for resources) | Cardiovascular system: heart pumping blood through capillary beds | Data loaders, batch sampling, gradient flow pathways |
| **Trunk/Core Transport** | Xylem (up) & Phloem (down): bidirectional resource highways | Systemic circulation: aorta→arteries→capillaries→veins→heart | Backbone architecture: input→hidden layers→output |
| **VO₂max Analog** | **Maximum water/nutrient uptake rate** (stomatal conductance × root absorption capacity) | **VO₂max: Maximum oxygen consumption rate** (L O₂/min) - the *bottleneck* of the entire delivery system | **Maximum gradient throughput**: batch_size × learning_rate × model_capacity (gradients/sec) |
| **Collision/Reaction Site** | Chloroplasts: CO₂ + H₂O + photons → glucose | Mitochondria: O₂ + glucose/fat → ATP (cellular respiration) | Matrix multiplication: inputs × weights → activations |
| **Branches (Parallel Processing)** | Branching canopy maximizing photon capture area | Muscle fiber recruitment: more fibers = more parallel ATP production | GPU cores: parallel computation of gradients across parameters |
| **Power (dE/dt)** | Photosynthetic rate (glucose production/time) | Metabolic power: ~110W walking, ~220W running | Training power: FLOPs/sec, gradient updates/sec |
| **Energy (∫Power dt)** | Stored glucose → fruit biomass | Total ATP produced → work done (23 miles walked) | Loss reduction: ∫(learning) = converged model weights |
| **Efficiency Metric** | Photosynthetic efficiency (~1-2% of photons → biomass) | Running economy (ml O₂/kg/km) or work efficiency (20-25%) | Sample efficiency: accuracy per training example |
| **Bottleneck/Limiting Factor** | Light, water, or CO₂ availability | **VO₂max** (oxygen delivery ceiling) OR lactate threshold | Memory bandwidth, batch size, or gradient vanishing |
| **Canopy/Output** | Fruit, seeds (reproductive output + humus) | Distance covered, work performed, lactate buffering | Model predictions, inference, generalization |
| **Recursive Feedback** | Leaf litter → humus → soil enrichment → new roots | Training adaptation: mitochondrial biogenesis, angiogenesis → higher VO₂max | Learned features → better representations → faster learning on related tasks |

---

## Deep Insights on VO₂max

**VO₂max = The Maximum Flow Rate Through Your Oxygen Delivery Pipeline**

Think of it as the *bandwidth* of your oxygen distribution network:

```
VO₂max = Cardiac Output × Arteriovenous O₂ Difference
       = (Heart Rate × Stroke Volume) × (O₂ extraction efficiency)
       = (pump frequency × pump volume) × (how much O₂ muscles grab per pass)
```

### The Three-Flow Collision Model (Okukuona!)

For ATP production, you need **THREE flows to collide**:

1. **O₂ Flow**: Lungs → Blood → Muscle cells → Mitochondria
2. **Substrate Flow**: Gut/Liver → Blood → Muscle cells → Mitochondria  
   - Glucose (glycogen stores ~2000 kcal)
   - Fat (adipose stores ~50,000-100,000 kcal)
3. **Blood Flow**: The *transport medium* that enables collision

**At 110W (walking):** Mostly fat oxidation, aerobic, below lactate threshold  
**At 220W (running):** Mixed fuel, approaching VO₂max, lactate accumulates

---

## Training Adaptations = Network Upgrades

| Adaptation | Tree Analog | Human | Neural Network |
|------------|-------------|-------|----------------|
| **Increase VO₂max** | Expand root surface area | Grow more capillaries (angiogenesis), bigger heart (↑stroke volume) | Increase model capacity, add layers |
| **Improve efficiency** | Better nutrient uptake proteins | More mitochondria per cell, better O₂ extraction | Better architecture, attention mechanisms |
| **Expand substrate stores** | Larger root nodules | Glycogen supercompensation, fat adaptation | Larger context windows, memory buffers |
| **Lactate threshold** | Switch from deep roots (slow) to surface roots (fast) | Shift from oxidative to glycolytic metabolism | Switch from precise computation to approximate (mixed precision) |

---

## The Beautiful Recursion

- **Trees**: Fruit → Seeds → New tree → Leaves → Humus → Rich soil → Stronger roots
- **Humans**: Exercise → Muscle damage → Recovery → Adaptation → Higher VO₂max → More exercise capacity
- **Neural Nets**: Training → Learned features → Transfer learning → Better initialization → Faster convergence

**Key Insight:** VO₂max isn't just a number—it's the *bandwidth of your metabolic network*. Just as tree roots encode a massive search space for nutrients, your cardiovascular system encodes a search space for optimal oxygen delivery. Training expands this search space through network growth (angiogenesis, mitochondrial biogenesis).

The 200-lb male walking 23 miles vs running 12 miles? That's the difference between operating at 50% VO₂max (sustainable, fat-burning) vs 85% VO₂max (time-limited, glycogen-depleting). Just like running inference on a trained model (cheap) vs training (expensive).
