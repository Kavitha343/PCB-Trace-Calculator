# PCB Trace Width & Current Capacity Calculator

A responsive, interactive web application built with vanilla HTML, CSS, and JavaScript. This tool utilizes industry-standard *IPC-2221 linear approximation formulas* to dynamically calculate optimal PCB trace widths for KiCad deployment based on current, copper thickness, and temperature limits.

## Features
- Real-time Calculations:Instant updates on input change without page refreshes.
- IPC-2221 Standard Engine:Separate calculation paths for External and Internal PCB layers.
- Safety Threshold Warnings:Visual indicator alerts when trace widths exceed standard manufacturing limits (5mm+).
- Fully Responsive Architecture:Optimized for both desktop workbenches and mobile devices.

## Tech Stack
- Frontend:HTML5, CSS3 (Custom Grid/Flexbox Layouts)
- Logic Engine:Vanilla JavaScript (ES6)

## The Core Formula Used
The application implements the standard IPC-2221 formula:
Area = (Current / (k * (TempRise^b))) ^ (1/c)
Width = Area / Thickness
