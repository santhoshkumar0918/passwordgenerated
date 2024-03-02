function generatePassword(length, includeLowerCase, includeUpperCase, includeNumbers, includeSymbol) {
    const lowerCaseChars = "abcdefghijklmnopqrstuvwxyz";
    const upperCaseChars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    const numbersChars = "0123456789";
    const symbolChars = "!@#$%^&*()_+";

    let allowedChars = "";
    let password = "";

    allowedChars += includeLowerCase ? lowerCaseChars : "";
    allowedChars += includeUpperCase ? upperCaseChars : "";
    allowedChars += includeNumbers ? numbersChars : "";
    allowedChars += includeSymbol ? symbolChars : "";

     if(length<=0){
        return`(password length must be 1)`
     }
     if(allowedChars.length === 0){
        return`(at least 1 set of charcters needs to be selected )`;
     }
     for(let i = 0; i < length;i++){
        const randomIndex = Math.floor(Math.random() *  allowedChars.length);
        password += allowedChars[randomIndex];
     }
 
         return password;
         }
         const passwordslength = 12;
         const includeUpperCase = true;
         const includeLowerCase = true;
         const includeNumbers = true;
         const includeSymbol = true;
      
         const password = generatePassword(passwordslength, 
                                         includeLowerCase,
                                         includeUpperCase,
                                         includeNumbers,
                                         includeSymbol);
         console.log(`Generated password: ${password}`);
