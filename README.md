# Susy Pong - Development Log

This file documents the iterative development of `susypong.html`, a simple Pong-like game, based on a series of requests.

## Feature Requests

1.  **Initial Game Creation** (Commit: `a4b195d`)
    *   Request: "Create a very basic minimal game of pong in plain javascript. No fancy graphics, just very basic keyboard or mouse control (you choose). Single-player."
    *   Implementation: A single-player Pong game with mouse-controlled paddle and a circular ball. Game ends if the ball goes past the paddle.

2.  **Ball Color Change** (Commit: `c3fa0c2`)
    *   Request: "Now make the ball pink please."
    *   Implementation: The ball's color was changed from red to pink.

3.  **Multiple Heart-Shaped Balls & Gameplay Modification** (Commits: `6e80e21`, `28b6d07`)
    *   Request: "Two balls please. And shaped like love hearts. And no game over when the ball escapes, just have it bounce off the bottom and game continues."
    *   Implementation:
        *   The game now features two balls.
        *   Balls are rendered as heart shapes.
        *   The "game over" condition was removed; balls now bounce off the bottom edge of the canvas.

4.  **Ball Duplication on Paddle Hit** (Commit: `f133a97`)
    *   Request: "Every time the ball hits the paddle, duplicate that ball, sending them in slightly different directions. Maximum 50 balls though."
    *   Implementation: When a heart hits the paddle, it duplicates, with the original and new heart moving off in slightly different directions. A maximum limit of 50 hearts was introduced.

5.  **Fading Rainbow Trails** (Commit: `7a5e464`)
    *   Request: "Can the hearts leave a fading rainbow trail behind them?"
    *   Implementation: Hearts now leave a trail of smaller, fading hearts behind them. Both the main hearts and their trails cycle through rainbow colors. A screen-clearing effect was modified to allow trails to fade gradually.
