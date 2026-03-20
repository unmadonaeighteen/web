উন্মাদনা ১৮ - Batch Frenzy Website 🎓Welcome to the উন্মাদনা ১৮ batch website project! This website is designed as a single, easily editable HTML file. You don't need a database or complex backend to update the content—everything is managed directly inside the index.html file.🚀 Quick StartTo view the website, simply double-click the index.html file to open it in any modern web browser (Chrome, Edge, Safari, Firefox).📝 How to Edit ContentAll the data for the website is stored at the bottom of the index.html file.Open index.html in any text editor (like VS Code, Notepad++, or standard Notepad), scroll down to the bottom, and look for the section labeled:// 1. EDITABLE DATABASE1. Adding a New Batchmate (Student Directory)Find the const studentsData = [ section. To add a new person, simply copy an existing block enclosed in { }, paste it inside the [ ], and change the details.Template:{
  nameBn: "নাম বাংলায়", nameEn: "Name in English",
  roleBn: "পেশা/পদবী", roleEn: "Profession/Role",
  orgBn: "প্রতিষ্ঠানের নাম", orgEn: "Organization Name",
  bloodGroup: "O+",
  addressBn: "ঠিকানা", addressEn: "Address",
  image: "LINK_TO_PHOTO",
  icon: "graduation-cap" // Options: briefcase, stethoscope, building-2, heart, user
}
Note: Make sure to separate multiple students with a comma ,!2. Adding Timeline EventsFind the const eventsData = [ section.Template:{
  dateBn: "তারিখ", dateEn: "Date",
  titleBn: "ইভেন্টের নাম", titleEn: "Event Title",
  descBn: "বিস্তারিত...", descEn: "Details...",
  isPast: false // Change to true if the event has already happened
}
3. Changing the Hero/Background Slider ImagesFind the const sliderImages = [ array. You can replace the URLs inside the quotation marks with your own image links.const sliderImages = [
  "[https://your-image-link-1.jpg](https://your-image-link-1.jpg)",
  "[https://your-image-link-2.jpg](https://your-image-link-2.jpg)",
  "[https://your-image-link-3.jpg](https://your-image-link-3.jpg)"
];
4. Updating Memory Categories (Photo Albums)Find the const memoryCategories = [ section. Here you can link to external photo albums (like Google Photos albums).Template:{ 
  badgeBn: "অ্যালবামের নাম", badgeEn: "Album Name", 
  image: "LINK_TO_COVER_PHOTO", 
  link: "LINK_TO_GOOGLE_PHOTOS_ALBUM" 
}
🌍 Changing Text & TranslationsIf you want to change static texts like section titles, button names, or footer text, look for:// 2. TRANSLATION DICTIONARYFind the const translations = { object. You can change the Bengali (bn) and English (en) text here."hero-title": { bn: "নতুন টাইটেল", en: "New Title" },
"footer-text": { bn: "© ২০২৬ · আপনাদের নাম", en: "© 2026 · Your Name" }
🎨 Changing General SettingsThe Background MusicPress Ctrl + F (or Cmd + F) and search for <audio id="bgm". Replace the src link with a link to your preferred .mp3 file.<source src="YOUR_MP3_LINK_HERE.mp3" type="audio/mpeg">
Theme ColorsIf you want to change the primary blue color, scroll to the top of the file to the <style> section and look for :root.Change the --accent variable::root {
  --accent: #0ea5e9; /* Change this hex code to your batch's theme color */
  /* ... */
}
Logo & FaviconTo change the logo, ensure your logo file is named Logo.svg and is in the same folder as index.html. If your logo is a .png or .jpg, search the HTML for Logo.svg and update it to match your filename.
