# tkw.github.io
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <script >
         let fullName = "Nguyen Minh Thu";
            let studentId = "27A4042989";
            let tenThuong = fullName.toLowerCase().split(" ");
            let tenChinh = tenThuong[tenThuong.length - 1];
            let tenHo = tenThuong[0];
            let tenDem = tenThuong[1];
            let vietTatHoTenDem = tenHo[0] + tenDem[0];
            let Email = `${tenChinh}${vietTatHoTenDem}.${studentId.toLowerCase()}@hvnh.edu.vn`;
             console.log(fullName,studentId);
            console.log("Email:",Email );
            let coursePeriod = studentId.substring(0, 2); 
      let facultyCode = studentId.substring(2, 6); 

      
      let faculties = {
          "A404": "Công nghệ thông tin & Kinh tế số",
         
      };
      let faculty = faculties[facultyCode] || "Khoa chưa xác định";

      let lastFourDigits = studentId.slice(-4); 
      let sum = 0;
      for (let digit of lastFourDigits) {
          sum += parseInt(digit);
      }

      
      console.log(`Xin chào ${fullName}, bạn là sinh viên khóa ${coursePeriod}, khoa ${faculty},tổng 4 số cuối trong mã sinh viên là ${sum}`)
    
        </script>
    </head>
    <body>
        
    </body>
    </html>
