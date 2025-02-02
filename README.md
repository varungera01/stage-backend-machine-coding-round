# Stage OTT Assignment: Implementation of MyList Feature and Optimizations in Other Functionalities

## Overview

This service manages a user's **My List**, allowing them to add, remove, and fetch their saved content (Movies/TV Shows). It also ensures optimized queries and scalability.

---

### Table of Contents

- [Overview](#overview)
- [Database Schema Changes](#database-schema-changes)
- [API Routes](#api-routes)
- [Author Info](#author-info)

---

## Database Schema Changes

### Schemas Introduced

- **User Schema**
- **UserContentPreference Schema**
- **MyList Schema**
- **UserWatchHistory Schema**

---

## API Routes

### **1. Get My List**
**Endpoint:** `GET /list`
- **Query Params:** `username`, `skip`, `limit`
- **Purpose:** Fetch paginated items from the user’s list with movie/TV show details.

### **2. Add to My List**
**Endpoint:** `POST /list`
- **Body:**
```json
{
  "username": "string",
  "contentId": "string",
  "contentType": "Movie" | "TVShow"
}
```
- **Purpose:** Adds an item to the user’s list.

### **3. Remove from My List**
**Endpoint:** `DELETE /list`
- **Body:**
```json
{
  "username": "string",
  "contentId": "string",
  "contentType": "Movie" | "TVShow"
}
```
- **Purpose:** Removes an item from the user’s list.

---


## Author Info

- LinkedIn - [Varun Gera](https://www.linkedin.com/in/varun-gera-6b922718b/)

