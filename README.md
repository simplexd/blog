# blog
学习记录
比较时间大小
function compareTime(time) {
      if(time) {
        var currentTime = (new Date()).valueOf();
        var plantTime = time.replace(/\-/g, "\/");
        var newPlantTime = new Date(plantTime);
        if (currentTime - newPlantTime > 0) {
          //时间未失效
          return false;
        } else {
          //时间失效
          return true;
        }
      }
    }
