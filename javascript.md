# trim函数
IE8以下不支持，需要手动编写

    if(!String.prototype.trim){
        String.prototype.trim = function(){
          var trimLeft = /^\s+/;
          var trimRight = /\s+$/; 
          return null==this?"":this.toString().replace( trimLeft, "" ).replace( trimRight, "" );
        };
      }

