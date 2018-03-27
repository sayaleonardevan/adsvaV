<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.2/jquery.mobile-1.4.2.min.css" />
<script src="http://code.jquery.com/jquery-1.9.1.min.js"></script>
<script src="http://code.jquery.com/mobile/1.4.2/jquery.mobile-1.4.2.min.js"></script>
</head>
<body>

    <div data-role="page" data-theme="a" id="index">
        <div data-role="header" data-position="inline">
            <h1>Calculator</h1>
        </div>
<div class="ui-field-contain">
    <label for="select-custom-1"></label>
    <select name="select-custom-1" id="select-custom-1" data-native-menu="false" >
        <option value="#index">factorial / pemangkatan calculator</option>
        <option value="#about">color hex</option>
        <option value="#services">Rangkuman Materi</option>
    </select>
    <script>
    $(function(){
     
      $('#select-custom-1').bind('change', function () {
          var url = $(this).val(); 
          if (url) { 
              $.mobile.changePage( url, { transition: "flip", changeHash: false });
          }
          return false;
      });
    });
</script>
</div>
        <div data-role="content" data-theme="a" >
       <h1>Pemangkatan</h1>
    <br>
    <input type="text" id=num placeholder="masukkan angka">
    <input type="text" id=parse placeholder="masukkan pangkat">
    <input type="text" id=hasil1 placeholder="hasil">
    <button onclick="pangkat()" data-textonly="false" data-textvisible="false" data-msgtext="" data-inline="true"> GO </button>
    
    <h1>Factorial</h1>
    <br>
    <input type="text" id=woi placeholder="masukkan angka">
    <input type="text" id=tole placeholder="hasil">
    <button onclick="faktorial()" data-textonly="false" data-textvisible="false" data-msgtext="" data-inline="true"> GO </button>
    <script>
  $(document).ready(function(){
  $('.target').on('change', function(){
  var url = $(this).val();
  window.location = url;
  });
});
function pangkat() {
      document.getElementById("hasil1").value = Math.pow(document.getElementById("num").value,document.getElementById("parse").value)
  };
  function faktorial() {
    document.getElementById("tole").value = 1
    for (i = 1; i <= document.getElementById("woi").value; i++) {
      document.getElementById("tole").value *= i
    };
    };
</script>
        </div>
        <div data-role="footer" data-theme="a">
        </div>
    </div>


    <div data-role="page" data-theme="a" id="about">
        <div data-role="header" data-position="inline">
            <h1>Color Hex to RGB</h1>
        </div>
<div class="ui-field-contain">
    <label for="select-custom-2"></label>
    <select name="select-custom-2" id="select-custom-2" data-native-menu="false">
        <option value="#index">factorial / pemangkatan calculator</option>
        <option value="#about" selected="selected">color hex</option>
        <option value="#services">Rangkuman Materi</option>
    </select>
    <script>
    $(function(){
      
      $('#select-custom-2').bind('change', function () {
          var url = $(this).val(); 
          if (url) { 
              $.mobile.changePage( url, { transition: "flip", changeHash: false });
          }
          return false;
      });
    });
</script>
</div>
        <div data-role="content" data-theme="a">
        <p> Masukkan Hex Input : </p>
        <input id="hexinput" type='text' class="pickedColor" type="text" placeholder="masukan hex" onkeyup="changeColor(this.className)" />
        
</br>
<input class="elementToChange" style="height:50px; width:100%; border:1px solid black" type="text"></input>
<script>
    function changeColor(className){
     document.getElementsByClassName("elementToChange")[0].style.background = document.getElementsByClassName(className)[0].value;
    }
</script>
<br />
<h1 id="results"></h1>
        </div>
<script>
function hexToRgba(hex) {
    var bigint, r, g, b, a
    var re = /^#?/;
    var aRgb = hex.replace(re, '');
    if (aRgb.length == 3) {
        bigint = parseInt(aRgb, 16);
        r = (bigint >> 4) & 255;
        g = (bigint >> 2) & 255;
        b = bigint & 255;
        return "rgba(" + r + "," + g + "," + b + ")";
    }
    if (aRgb.length == 6) {
        bigint = parseInt(aRgb, 16);
        r = (bigint >> 16) & 255;
        g = (bigint >> 8) & 255;
        b = bigint & 255;
        return "rgba(" + r + "," + g + "," + b + ")";
    }
    if (aRgb.length == 8) {
        bigint = parseInt(aRgb, 16);
        a = ((bigint >> 24) & 255) / 255;
        r = (bigint >> 16) & 255;
        g = (bigint >> 8) & 255;
        b = bigint & 255;
        return "rgba(" + r + "," + g + "," + b + "," + a.toFixed(1) + ")";
}

}

$('#hexinput').on('input', function () {
    $('#results').text(hexToRgba($('#hexinput').val()));
});
$('#myTextbox1').on('input', function () {
    alert('Text1 changed!');
});

</script>
</div>
        <div data-role="footer" data-theme="a">
        </div>
    </div>

    
    <div data-role="page" data-theme="a" id="services">
        <div data-role="header" data-position="inline">
            <h1>Rangkuman Materi</h1>
        </div>
<div class="ui-field-contain">
    <label for="select-custom-3"></label>
    <select name="select-custom-3" id="select-custom-3" data-native-menu="false">
        <option value="#index">factorial / pemangkatan calculator</option>
        <option value="#about">color hex</option>
        <option value="#services" selected="selected">Rangkuman Materi</option>
    </select>
<script>
    $(function(){
      
      $('#select-custom-3').bind('change', function () {
          var url = $(this).val(); 
          if (url) { 
              $.mobile.changePage( url, { transition: "flip", changeHash: false });
          }
          return false;
      });
    });
</script>
        <div data-role="content" data-theme="a">
        <h1>Rangkuman Materi PPM</h1>
        <ul data-role="listview">
    <li><p>1. pada pertemuan pertama kami di ajarkan mengenai perkembangan mobile dari jaman 1G sampai pada 4G</p></li>
    <li><p>2. pada pertemuan kedua kami disuruh untuk membuat rangkuman github : <br> 
1. git init : untuk inisialisasi git<br>
2. git status : untuk mengecek state dari suatu project<br>
    jika file sudah masuk staging area menjadi changes to be made<br>
3. git add octocat.txt : membuat file octocat.txt<br>
4. git commit-m "Add cute octocat story" : menyimpan "Add cute octocat story" di dalam file<br>
5. git add '*.txt' : memasukan semua file ke dalam git (staging area)<br>
6. git commit -m 'Add all the octocat txt files' : mengganti semua isi file karena semua file telah dimasukan ke staging area<br>
7. git log : semua tindakan yang pernah dilakukan<br>
8. git remote add origin https://github.com/try-git/try_git.git : menambah remote repository<br>
9. git push -u origin master : untuk mengirim data dari local ke server<br>
10.git pull origin master : untuk melihat apa yang telah diganti pada file kita<br>
11.git diff HEAD : untuk mengecek perbedaan yang telah di buat , HEAD untuk melihat yang terakhir di commit<br>
12.git add octofamily/octodog.txt : memasukan octodog.txt di dalam octofamily ke dalam staging<br>
13.git diff --staged : untuk melihat apa yang telah kita rubah<br>
14.git reset octofamily/octodog.txt : untuk unstage octofamily/octodog.txt<br>
15.git checkout -- octocat.txt : mengganti octocat.txt ke commit terakhir<br>
16.git branch clean_up : membuat branch<br>
17.git checkout clean_up : untuk pindah branch<br>
18.git rm '*.txt': mengahpus file (semua karena menggunakan nama '*.txt')<br>
19.git commit -m "remove all the cats" : untuk memastikan untuk menghapus<br>
20.git checkout master : pinda ke branch master<br>
21.git merge clean_up : untuk menggabungkan branch<br>
22.git branch -d clean_up : menghapus branch clean_up23.git push : mengirim semua perubahan ke server<br>
</p></li>
    <li><p>3. pada pertemuan ke 3 , kita di ajarkan basic dari jquery mobile dan melakukan latihan jquery mobile sederhana</p></li>
    <li><p>4. pada pertemuan ke 4 , kita di ajarkan angular</p></li>
</ul>
<br>
<input type="range" name="slider-1" id="slider-1" value="60" min="0" max="100" />
        </div>
        <div data-role="footer" data-theme="a">
        </div>
<a href="#popupBasic" data-rel="popup" class="ui-btn ui-corner-all ui-shadow ui-btn-inline" data-transition="pop">click me!</a>
<div data-role="popup" id="popupBasic">
<p>me!me!me!me!me!me!</p>
</div>
<table data-role="table" id="table-custom-2" data-mode="columntoggle" class="ui-body-d ui-shadow table-stripe ui-responsive" data-column-btn-theme="b" data-column-btn-text="Columns to display..." data-column-popup-theme="a">
    <thead>
      <tr class="ui-bar-d">
        <th data-priority="2">Rank</th>
        <th>Movie Title</th>
        <th data-priority="3">Year</th>
        <th data-priority="1"><abbr title="Rotten Tomato Rating">Rating</abbr></th>
        <th data-priority="5">Reviews</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th>1</th>
        <td><a href="http://en.wikipedia.org/wiki/Citizen_Kane" data-rel="external">Citizen Kane</a></td>
        <td>1941</td>
        <td>100%</td>
        <td>74</td>
      </tr>
      <tr>
        <th>2</th>
        <td><a href="http://en.wikipedia.org/wiki/Casablanca_(film)" data-rel="external">Casablanca</a></td>
        <td>1942</td>
        <td>97%</td>
        <td>64</td>
      </tr>
      <tr>
        <th>3</th>
        <td><a href="http://en.wikipedia.org/wiki/The_Godfather" data-rel="external">The Godfather</a></td>
        <td>1972</td>
        <td>97%</td>
        <td>87</td>
      </tr>
      <tr>
        <th>4</th>
        <td><a href="http://en.wikipedia.org/wiki/Gone_with_the_Wind_(film)" data-rel="external">Gone with the Wind</a></td>
        <td>1939</td>
        <td>96%</td>
        <td>87</td>
      </tr>
      <tr>
        <th>5</th>
        <td><a href="http://en.wikipedia.org/wiki/Lawrence_of_Arabia_(film)" data-rel="external">Lawrence of Arabia</a></td>
        <td>1962</td>
        <td>94%</td>
        <td>87</td>
      </tr>
      <tr>
        <th>6</th>
        <td><a href="http://en.wikipedia.org/wiki/Dr._Strangelove" data-rel="external">Dr. Strangelove Or How I Learned to Stop Worrying and Love the Bomb</a></td>
        <td>1964</td>
        <td>92%</td>
        <td>74</td>
      </tr>
      <tr>
        <th>7</th>
        <td><a href="http://en.wikipedia.org/wiki/The_Graduate" data-rel="external">The Graduate</a></td>
        <td>1967</td>
        <td>91%</td>
        <td>122</td>
      </tr>
      <tr>
        <th>8</th>
        <td><a href="http://en.wikipedia.org/wiki/The_Wizard_of_Oz_(1939_film)" data-rel="external">The Wizard of Oz</a></td>
        <td>1939</td>
        <td>90%</td>
        <td>72</td>
      </tr>
      <tr>
        <th>9</th>
        <td><a href="http://en.wikipedia.org/wiki/Singin%27_in_the_Rain" data-rel="external">Singin' in the Rain</a></td>
        <td>1952</td>
        <td>89%</td>
        <td>85</td>
      </tr>
      <tr>
        <th>10</th>
        <td class="title"><a href="http://en.wikipedia.org/wiki/Inception" data-rel="external">Inception</a></td>
        <td>2010</td>
        <td>84%</td>
        <td>78</td>
      </tr>
    </tbody>
  </table>
    </div>
</body>
</html>
