<p>
	<a href="https://keenthemes.com/metronic">
		<img src="https://keenthemes.com/static/metronic/tailwind/docs/dist/assets/media/app/default-logo.svg" alt="Metronic"/>
	</a>
</p>

## Setup example
### Copy Source Folder

- Copy the `src` folder from the `metronic-tailwind-html` package and paste it into the React `src` directory.


- Rename the copied folder to `metronic` so that the directory structure should now look like this: `src/metronic`. This step imports the necessary styles and assets from the original HTML package into your React project.


- In the `src/metronic/core` folder, delete the unnecessary `index.ts` file. This file is not needed for Single Page Application (SPA) integration as it could cause conflicts. Instead, rename the `index.spa.ts` file to `index.ts` to ensure proper integration.


- Replace HTML initialization with default instance export in `src/metronic/app/layouts/demo1.js`.

    Replace the code part below:

    ```javascript
    KTDom.ready(() => {
        KTLayout.init();
    });
    ```
    with
    ```javascript
    export default KTLayout;
    ```

### Copy Media Folder

 - Copy the `media` folder from the `metronic-tailwind-html` package's `dist/assets/media` directory into your React project's `public` directory.

### Install Packages & Start Development Server

- Install the required Node.js packages by running `npm install`. Start the React development server by running `npm run dev`.
