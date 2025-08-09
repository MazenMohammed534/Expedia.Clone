## Expedia.com System – Backend Implementation
A simplified backend system inspired by Expedia.com, focusing on flight and hotel booking functionalities with integrated payment processing.
This project demonstrates several software design principles and patterns applied in a travel booking context.

---

## ✨ Key Features
**Multi-service Integration** – Connects with multiple airline and hotel APIs

**Reservation Management** – Handles complex itineraries with flights and hotels

**Payment Processing** – Supports multiple payment providers (PayPal, Stripe, Square)

**User Management** – Customer profiles with payment methods and booking history

**Error Handling** – Transaction-like rollback for failed reservations

---

## 🏗 System Architecture
The system follows a layered architecture with clear separation of concerns:

**Frontend Layer** – ExpediaFrontend handles user interactions

**Business Logic Layer** – CustomerManager and ExpediaBackend manage core operations

**Service Layer** – Interfaces with external APIs (flights, hotels, payments)

**Data Layer** – Simple in-memory storage (for demonstration purposes)

---

## 🎯 Design Patterns Used
**Factory Pattern** – FlightsFactory, HotelsFactory, PaymentFactory create service instances

**Adapter Pattern** – SquarePayment adapts JSON-based API

**Strategy Pattern** – Multiple payment providers implement a common interface

**Composite Pattern** – ItineraryReservation treats individual and composite reservations uniformly

**Prototype Pattern** – Clone() method for reservation duplication

