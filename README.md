OVERVIEW:

This project seeks to model a 1-D transient thermal hydraulic model of a liquid cooling in a cylindrical pipe with internal heat generation and convective heat loss to the surrounding environment. The model solves an axial energy balance using heat transfer and fluid flow relations, discretized into axial control volumes and integrated using Euler's Method. The goal of this project is to build an understanding for systems-level thermal hydraulic behavior.

PHYSICAL SYSTEMS:
- Single cylindrical pipe
- Liquid sodium coolant
- Axial plug flow scheme (1-D)
- Uniform volumetric heat generation
- Convective heat loss from the pipe surface area to the surrounding environment

  This type of model relates to concepts in:
  - Reactor coolant channels
  - heat exchanger flows
  - thermal hydraulic analysis

METHODS:
- Spatial discretization:
    - Finite volumes
    - Uniform axial nodes
    - Upwind differencing for convective transport
- Time integration:
    - Forward Euler method
    - Fixed step in time
- Boundary condition:
    - Defined inlet temperature
    - Natural outflow at outlet

  Note: The model currently progresses the time in increments until a definied stopping point. Further versions of the model will detect steady state conditions and automatically stop.


KEY ASSUMPTIONS: 
- One-dimensional axial flow (no radial gradients)
- Constant thermophysical properties
- No axial conduction
- No pressure drop
- No momentum change
- Single-phase liquid flow
- Constant heat transfer coefficient

The intention of these assumptions are to isolate core thermal hydraulic behvaiors.


RESULTS:
This model can produce:
- Axial temperature profiles along the pipe
- Transient temperature evolution over time
- identification of peak temperature nodes

PROJECT MOTIVATION:
This project was developed to:
- Strengthen understanding of thermal hydraulic system modeling
- Gain experience with time integration
- Build intuition for reactor flow and heat transfer behavior
- Create a model that can be expanded to include more advanced analyses

Future developments for this project could include temperature depenedent properties, flow transients, and steady-state detection.
