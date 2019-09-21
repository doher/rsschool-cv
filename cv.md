# Aliaksandr Pletsiazhou

## Contact Info

* **MOB.:** +375 29 860-60-95
* **E-MAIL:** alexandr.pletezhov@gmail.com
* **CITY:** Minsk
* **LN:** in/a-pletsiazhou

## Summary

I am a calm, purposeful person who easily joins the team, is highly motivated to achieve success in the desired area. My goal is to find or develop an interesting project that could help people in their daily routine.

## Skills

* **Programming Languages:**  ​Javascript(ES5/ES6), HTML5, CSS3, TypeScript
* **Libraries:**  JQuery, Pixijs, Howlerjs
* **IDE:** VS Code, Sublime Text 3
* **Version Control:** Git, SVN

## Code Examples

```javascript
'use strict';

export const MAX_RADIUS = 20;

export class BallController {
    constructor() {
        let _model;
    }

    start(model) {
        this._model = model;
    }

    expandBall() {
        let model = this._model,
            radius = model.getRadius(),
            speed = model.getSpeed();

        radius = ((radius + speed) < 0) ? 0 : (radius + speed);

        if (radius >= MAX_RADIUS) {
            model.setSpeed(-speed);
        }

        model.setRadius(radius);
        model.updateView();
    }
}
```

```javascript
'use strict';

export class BallModel {
    constructor(x, y, radius = 1, speed = 0.3) {
        let _x = x,
            _y = y,
            _radius = radius,
            _speed = speed,
            _view;

        this.getX = function () {
            return _x;
        }

        this.getY = function () {
            return _y;
        }

        this.getRadius = function () {
            return _radius;
        }

        this.setRadius = function (radius) {
            _radius = radius;
        }

        this.getSpeed = function () {
            return _speed;
        }

        this.setSpeed = function (speed) {
            _speed = speed;
        }
    }

    start(view) {
        this._view = view;
    }

    updateView() {

        if (this._view) {
            this._view.update();
        }
    }
}
```

## Experience
* Wrote [Clicker-Game](https://github.com/doher/Clicker-Game) project  on the development of click skill, using JQuery, AJAX, MVC
* Wrote [Slot-Machine]( https://doher.github.io/slot-game/), using TypeScript, Pixijs, MVC, Howlerjs

## Education
* **EDUCATIONAL CENTER OF HIGH-TECH PARK  (11/2018 - 03/2019)** Student. Front-end web development
* **BELARUSIAN NATIONAL TECHNICAL UNIVERSITY (2006 - 2012)** M. Sc. Mechanical Engineering. Integrated Sensor-Based System. Received a master's degree

## English
* Pre-Intermediate+ (3 year in Polyglot school)