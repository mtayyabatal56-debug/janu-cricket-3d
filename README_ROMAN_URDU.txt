JANU CRICKET 3D - APK BUILD

1) Is folder ko GitHub par new repository mein upload karein.
2) GitHub repo mein Actions tab kholein.
3) 'Build Janu Cricket 3D APK' workflow select karein.
4) 'Run workflow' dabayein.
5) Build green/success hone par workflow run kholein.
6) Neeche Artifacts mein Janu-Cricket-3D-APK download karein.
7) ZIP extract karke app-debug.apk install karein.

TERMUX se GitHub par bhejne ke liye:
pkg update -y
pkg install git gh python -y
gh auth login

Project folder mein ja kar:
gh repo create janu-cricket-3d --public --source=. --remote=origin --push

Phir GitHub website > repo > Actions > Build Janu Cricket 3D APK > Run workflow.

NOTE: APK GitHub Actions ke cloud Linux runner par compile hota hai. Termux/Python project upload aur manage karte hain. HTML assets APK ke andar bundled hain; external internet dependency nahi honi chahiye.
