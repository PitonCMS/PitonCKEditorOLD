# PitonCMS CKEditor5 Custom Build

Custom build of CKEditor5 for PitonCMS, based on the Classic build. Includes custom media image management to select saved media files in PitonCMS to insert into the document editor.

This bundle started with a copy of the classic build packge from https://github.com/ckeditor/ckeditor5/tree/master/packages/ckeditor5-build-classic.

## Installing and Modifying
Clone this repo to your local development environment and navigate into the new project.
```
git clone git@github.com:PitonCMS/PitonCKEditor.git
cd PitonCKEditor
```

Initialize NPM so that `package.json` is updated automatically when adding package dependencies, just accept default prompts.
```
npm init
```

Install node dependencies, this may take a while...
```
npm install
```


To add a new CKEditor plugin, request it within the project.
```
npm install --save <package-name>
```

When finished, _build_ a new version of Piton CKEditor to compile the source into a single ckeditor.js file with translations.
```
npm run build
```

Then copy the finished `build` directory into PitonCMS/Engine/assets/ckeditor5/ and commit to `PitonCMS/Engine`.
