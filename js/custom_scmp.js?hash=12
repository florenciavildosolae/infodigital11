jQuery(document).ready(function ($) {
    $(".stickyLinks").delay(3000).fadeIn(1000); // FIXED LINKS
    
    var o=$("video").not("[ autoplay ]"),t=200;$(document).on("scroll",function(){var i=$(window).scrollTop()+t,n=$(window).scrollTop()+$(window).height()-t;o.each(function(o,t){var a=$(this).offset().top,e=$(this).height()+a;i<e&&n>a?$(this).get(0).play():$(this).get(0).pause()})}) // AUTOPLAY VIDEO ON SCROLL*/
    
    $('ul.choose li').click(function(){
		var tab_id = $(this).attr('data-tab');

		$('ul.choose li').removeClass('current');
		$('.tab-content').removeClass('current');

		$(this).addClass('current');
		$("#"+tab_id).addClass('current');
	})

    $(window).on("contextmenu",function(){return false;});
    
    if(window.location.protocol != 'https:') {
      location.href =   location.href.replace("http://", "https://");
    }
    
});
/*-------------------------------------------------------------------------------LEFT SIDE MENU--------------------------------- */
function openMenu() {
    var e = document.getElementById("leftmenu");
    if (e.style.width == '280px') {
        e.style.width = '0px';
    }
    else {
        e.style.width = '280px';
    }
}
/*-------------------------------------------------------------------------------HIDE OPTION ON SCROLL-------------------------- */
var scrollDown = 0;
$(window).scroll(function (event) {
    var up = $(this).scrollTop();
    if (up > scrollDown) {
        $('.stickyLinks').removeClass('active');
    }
    else {
        $('.stickyLinks').addClass('active');
    }
    scrollDown = up;
    var scroll = $(window).scrollTop();
    if (scroll >= 200) {
        $(".stickyLinks").addClass("hidden");
    }
    else {
        $(".stickyLinks").removeClass("hidden");
    }
});

/*-------------------------------------------------------------------------------BUTTONS-------------------------- */

/* VIDEO DIAGRAMS */

var vid = document.getElementById("video01");
vid.ontimeupdate = function () {
    myFunction()
};

function myFunction() {
    if ((vid.currentTime >= 2) && (vid.currentTime <= 6.5)) {
        document.getElementById('over01').style.opacity = '1';
    } else {
        document.getElementById('over01').style.opacity = '0';
    }
}

var vidtwo = document.getElementById("video02");
vidtwo.ontimeupdate = function () {
    myFunctiontwo()
};

function myFunctiontwo() {
    if ((vidtwo.currentTime >= 1) && (vidtwo.currentTime <= 4)) {
        document.getElementById('over02').style.opacity = '1';
    } else {
        document.getElementById('over02').style.opacity = '0';
    }
}

var vidthree = document.getElementById("video03");
vidthree.ontimeupdate = function () {
    myFunctionthree()
};

function myFunctionthree() {
    if ((vidthree.currentTime >= 2) && (vidthree.currentTime <= 6)) {
        document.getElementById('over03').style.opacity = '1';
    } else {
        document.getElementById('over03').style.opacity = '0';
    }
}

var vidfour = document.getElementById("video04");
vidfour.ontimeupdate = function () {
    myFunctionfour()
};

function myFunctionfour() {
    if ((vidfour.currentTime >= 1) && (vidfour.currentTime <= 7)) {
        document.getElementById('over04').style.opacity = '1';
    } else {
        document.getElementById('over04').style.opacity = '0';
    }
}

var vidfive = document.getElementById("video05");
vidfive.ontimeupdate = function () {
    myFunctionfive()
};

function myFunctionfive() {
    if ((vidfive.currentTime >= 2) && (vidfive.currentTime <= 7)) {
        document.getElementById('over05').style.opacity = '1';
    } else {
        document.getElementById('over05').style.opacity = '0';
    }
}


/* AUDIO */

var audioElement = new Audio('audio/mtr-announce.mp3');

$('.play').on('click', function() {
  $(this).hide();
  $('.pause').css('display', 'inline-block');
  audioElement.play();
});

$('.pause').on('click', function() {
  $(this).hide();
  $('.play').css('display', 'inline-block');
  audioElement.pause();
});

/* NO DRAG */

function absorbEvent_(event) {
            var e = event || window.event;
            e.preventDefault && e.preventDefault();
            e.stopPropagation && e.stopPropagation();
            e.cancelBubble = true;
            e.returnValue = false;
            return false;
        }

        function preventLongPressMenu(node) {
            node.ontouchstart = absorbEvent_;
            node.ontouchmove = absorbEvent_;
            node.ontouchend = absorbEvent_;
            node.ontouchcancel = absorbEvent_;
        }

        function init() {
            preventLongPressMenu(document.getElementById('theimage'));
        }