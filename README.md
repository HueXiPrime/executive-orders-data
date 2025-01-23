# Trump Executive Orders Data Repository

Welcome to the dedicated **data-only** repository for the Trump Executive Order Tracker.  
Here, we maintain the canonical `executive-orders.json` file and related documentation so that any interested party can contribute new or updated Executive Order (EO) information.

**Why a separate data repository?**  
Splitting the data from front-end code keeps everything clean and consistent— everyone can use this data in any interface they’d like while ensuring there's a single source of truth.

---

## How to Use This Repository

1. **Clone or Fork** this repository to gain access to `executive-orders.json`.
2. Integrate the JSON data into your own project or front-end.
3. When new EOs appear—or existing entries need updating—either open a Pull Request directly or log an Issue (see [Contributing](#contributing)).

---

## Data Structure

Each entry in `executive-orders.json` contains:

- **title**: The official or commonly recognized title of the EO.
- **documentLink**: Link to the official document (e.g., the Federal Register).
- **summary**: A short, factual summary (max 200 characters).
- **currentStatus**: Where the EO stands in the implementation process.
- **dateSigned**: The date the order was signed by the President.
- **implementationNotes**: Additional info on how the EO is being carried out.
- **knownLawsuits**: Details on any legal challenges.
- **impactForecast**: (Optional) High-level assessment of the potential effect.
- **stallProbability**: (Optional) Probability or risk factor that it gets delayed or blocked.

Feel free to add optional fields if needed, but keep the above fields as your minimum baseline.

---

## Contributing

We welcome contributions from anyone who wants to keep this data accurate and up-to-date!

### 1. Via GitHub Pull Requests (Recommended)

1. Fork this repository.
2. Make your changes to [`executive-orders.json`](./executive-orders.json).
3. Submit a Pull Request describing what you changed or added.

### 2. Via GitHub Issues

If you aren’t comfortable editing JSON directly:

1. [Create an Issue](../../issues/new) outlining your suggested change.
2. Include as much detail as possible (sources, official links, etc.).

---

## Contribution Guidelines

1. **Objective, Factual Summaries**  
   Avoid personal commentary or political bias.
2. **Official Sources**  
   Always try to link to official government pages or court documents for lawsuits.
3. **Date and Status Updates**
   - Use `"Unclear"` if the implementation status is uncertain.
   - Mark `"Blocked"` only with an official court order.
   - Use `"Implementation in progress"` for partial rollouts.
   - Update the `lastUpdated` (if applicable) whenever you modify an EO entry.

---

## Example Projects Using This Data

Here are some repositories that utilize this dataset:

- [Trump Executive Order Tracker](https://github.com/HueXiPrime/Trump-Executive-Order-Tracker) - Huexi's Interface
- [Trump EOs Tracker](https://github.com/kaushika05/trump-eos-tracker) - Kaushika's Interface
