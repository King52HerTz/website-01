    function animate(obj, target, callback) {
        clearInterval(obj.timer);
        obj.timer = setInterval(function() {
            var speed = (target - obj.offsetLeft) / 10;
            // 判断speed正负，不同方向取整
            var speed1 = speed > 0 ? Math.ceil(speed) : Math.floor(speed);
            if (obj.offsetLeft == target) {
                clearInterval(obj.timer);
                callback && callback();
            }
            obj.style.left = obj.offsetLeft + speed1 + 'px';

        }, 15);
    };