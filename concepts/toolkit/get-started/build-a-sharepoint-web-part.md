---
title: Создание веб-части SharePoint с помощью microsoft Graph набор средств
description: Начало работы с использованием microsoft Graph набор средств для создания веб-части SharePoint.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d07a597c69ae998c75e3d4698cb0513cff056e56
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659752"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="01e00-103">Создание веб-части SharePoint с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="01e00-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="01e00-104">В этом разделе описывается, как использовать набор средств Microsoft Graph в клиентской [веб-части SharePoint.](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)</span><span class="sxs-lookup"><span data-stu-id="01e00-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="01e00-105">Начало работы состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="01e00-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="01e00-106">Настройка среды разработки и создание веб-части.</span><span class="sxs-lookup"><span data-stu-id="01e00-106">Set up your development environment and create a web part.</span></span>
2. <span data-ttu-id="01e00-107">Обновите TypeScript в проекте.</span><span class="sxs-lookup"><span data-stu-id="01e00-107">Update TypeScript in your project.</span></span>
3. <span data-ttu-id="01e00-108">Добавьте microsoft Graph набор средств.</span><span class="sxs-lookup"><span data-stu-id="01e00-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="01e00-109">Добавьте поставщика SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01e00-109">Add the SharePoint Provider.</span></span>
5. <span data-ttu-id="01e00-110">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="01e00-110">Add components.</span></span>
6. <span data-ttu-id="01e00-111">Настройка разрешений.</span><span class="sxs-lookup"><span data-stu-id="01e00-111">Configure permissions.</span></span>
7. <span data-ttu-id="01e00-112">Создайте и разверните веб-часть.</span><span class="sxs-lookup"><span data-stu-id="01e00-112">Build and deploy your web part.</span></span>
8. <span data-ttu-id="01e00-113">Протестировать веб-часть.</span><span class="sxs-lookup"><span data-stu-id="01e00-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="01e00-114">Настройка среды разработки SharePoint Framework и создание новой веб-части</span><span class="sxs-lookup"><span data-stu-id="01e00-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="01e00-115">Выполните действия, [чтобы настроить среду разработки SharePoint Framework,](/sharepoint/dev/spfx/set-up-your-development-environment) а затем [создайте новую веб-часть.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)</span><span class="sxs-lookup"><span data-stu-id="01e00-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="update-typescript-in-your-project"></a><span data-ttu-id="01e00-116">Обновление TypeScript в проекте</span><span class="sxs-lookup"><span data-stu-id="01e00-116">Update TypeScript in your project</span></span>

<span data-ttu-id="01e00-117">Для набор средств Microsoft Graph требуется Typescript 3.x.</span><span class="sxs-lookup"><span data-stu-id="01e00-117">The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="01e00-118">Перед добавлением набор средств в проект убедитесь, что вы используете поддерживаемую [версию Typescript.](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)</span><span class="sxs-lookup"><span data-stu-id="01e00-118">Before adding the Toolkit to your project, make sure you're using a [supported version of Typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span> <span data-ttu-id="01e00-119">Например, чтобы добавить Typescript 3.7, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="01e00-119">For example, to add Typescript 3.7, use the following command:</span></span>

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
<span data-ttu-id="01e00-120">Затем найдите файл в папке проекта, откройте файл и найдите `tsconfig.json` эту строку:</span><span class="sxs-lookup"><span data-stu-id="01e00-120">Then, locate the `tsconfig.json` file in your project folder, open the file, and look for this line:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
<span data-ttu-id="01e00-121">Замените строку на:</span><span class="sxs-lookup"><span data-stu-id="01e00-121">Replace the line with:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="01e00-122">Добавление учетной записи Microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="01e00-122">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="01e00-123">Установите пакет и набор средств npm Microsoft Graph с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="01e00-123">Install the Microsoft Graph Toolkit npm package and polyfills with the following command:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="01e00-124">Если вы планируете поддерживать IE11 в веб-частях, вам потребуется предпринять дополнительные действия, чтобы обеспечить совместимость между браузерами:</span><span class="sxs-lookup"><span data-stu-id="01e00-124">If you plan to support IE11 in your web parts, you'll need to follow additional steps to ensure cross-browser compatibility:</span></span>

1. <span data-ttu-id="01e00-125">Установите следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="01e00-125">Install the following packages:</span></span>
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. <span data-ttu-id="01e00-126">Добавьте следующий код в `gulpfile.js` , прямо `build.initialize(gulp)` над:</span><span class="sxs-lookup"><span data-stu-id="01e00-126">Add the following code to `gulpfile.js`, right above `build.initialize(gulp)`:</span></span>
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```
3. <span data-ttu-id="01e00-127">В `src\webparts\<your-project>\<your-web-part>.ts` файле импортировать следующие полифайли перед поставщиком SharePoint на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="01e00-127">In your `src\webparts\<your-project>\<your-web-part>.ts` file, import the following polyfills before the SharePoint provider in the next step.</span></span>

```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="01e00-128">Добавление поставщика SharePoint</span><span class="sxs-lookup"><span data-stu-id="01e00-128">Add the SharePoint Provider</span></span>

<span data-ttu-id="01e00-129">Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="01e00-129">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="01e00-130">Дополнительные узнать [см. в этой теме.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="01e00-130">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="01e00-131">Веб-части SharePoint всегда существуют в контексте с проверкой подлинности, так как пользователю уже пришлось войти на страницу, на которую размещена веб-часть.</span><span class="sxs-lookup"><span data-stu-id="01e00-131">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="01e00-132">Используйте этот контекст для инициализации [поставщика SharePoint.](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="01e00-132">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="01e00-133">Сначала добавьте поставщика в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="01e00-133">First, add the provider to your web part.</span></span> <span data-ttu-id="01e00-134">Найдите файл в папке проекта и добавьте следующую строку в верхнюю часть файла `src\webparts\<your-project>\<your-web-part>.ts` под существующими `import` строками:</span><span class="sxs-lookup"><span data-stu-id="01e00-134">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

<span data-ttu-id="01e00-135">Затем необходимо инициализировать поставщика с контекстом проверки подлинности в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="01e00-135">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="01e00-136">В том же файле добавьте следующий код прямо перед `public render(): void {` строкой:</span><span class="sxs-lookup"><span data-stu-id="01e00-136">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a><span data-ttu-id="01e00-137">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="01e00-137">Add components</span></span>

<span data-ttu-id="01e00-138">Теперь можно приступить к добавлению компонентов в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="01e00-138">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="01e00-139">Просто добавьте компоненты в HTML-код внутри метода, и компоненты будут использовать контекст SharePoint для доступа `render()` к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="01e00-139">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="01e00-140">Например, чтобы добавить компонент [Person,](../components/person.md)код будет выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="01e00-140">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="01e00-141">Настройка разрешений</span><span class="sxs-lookup"><span data-stu-id="01e00-141">Configure permissions</span></span>

<span data-ttu-id="01e00-142">Чтобы вызвать Microsoft Graph из приложения SharePoint Framework, необходимо запросить необходимые разрешения в пакете решения, а администратор клиента Microsoft 365 должен утвердить запрашиваемую.</span><span class="sxs-lookup"><span data-stu-id="01e00-142">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="01e00-143">Чтобы добавить разрешения в пакет решения, найдите и откройте `config\package-solution.json` файл и установите:</span><span class="sxs-lookup"><span data-stu-id="01e00-143">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="01e00-144">Под этой строкой добавьте следующее:</span><span class="sxs-lookup"><span data-stu-id="01e00-144">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="01e00-145">Определите необходимые разрешения API Microsoft Graph в зависимости от используемого компонента.</span><span class="sxs-lookup"><span data-stu-id="01e00-145">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="01e00-146">На странице документации каждого компонента содержится список разрешений, необходимых компоненту.</span><span class="sxs-lookup"><span data-stu-id="01e00-146">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="01e00-147">Вам потребуется добавить каждое разрешение, необходимое для `webApiPermissionRequests` .</span><span class="sxs-lookup"><span data-stu-id="01e00-147">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="01e00-148">Например, если вы используете компонент "Человек" и "Повестка дня", ваши задачи `webApiPermissionRequests` могут выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="01e00-148">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

```json
"webApiPermissionRequests": [
  {
    "resource": "Microsoft Graph",
    "scope": "User.Read"
  },
  {
    "resource": "Microsoft Graph",
    "scope": "Calendars.Read"
  }
]
```
## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="01e00-149">Создание и развертывание веб-части</span><span class="sxs-lookup"><span data-stu-id="01e00-149">Build and deploy your web part</span></span>

<span data-ttu-id="01e00-150">Теперь вы создайте приложение и развернем его в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01e00-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="01e00-151">Создайте приложение с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="01e00-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="01e00-152">В `sharepoint/solution` папке будет новый `.sppkg` файл.</span><span class="sxs-lookup"><span data-stu-id="01e00-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="01e00-153">Вам потребуется отправить этот файл в каталог приложений SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="01e00-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="01e00-154">Перейдите на [страницу "Дополнительные функции" в Центре администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="01e00-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="01e00-155">Выберите **"Открыть** в **приложениях",** затем **"Каталог приложений"** и **"Распространение приложений для SharePoint".**</span><span class="sxs-lookup"><span data-stu-id="01e00-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="01e00-156">Загрузите `.sppkg` файл и нажмите кнопку **"Развернуть".**</span><span class="sxs-lookup"><span data-stu-id="01e00-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="01e00-157">Затем необходимо утвердить разрешения от администратора.</span><span class="sxs-lookup"><span data-stu-id="01e00-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="01e00-158">Перейдите в **Центр администрирования SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="01e00-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="01e00-159">В области навигации слева выберите **"Расширенный",** а затем **"Доступ к API".**</span><span class="sxs-lookup"><span data-stu-id="01e00-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="01e00-160">Должны отложенные запросы для каждого из разрешений, добавленных в `config\package-solution.json` файл.</span><span class="sxs-lookup"><span data-stu-id="01e00-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="01e00-161">Выберите и утвердит каждое разрешение.</span><span class="sxs-lookup"><span data-stu-id="01e00-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="01e00-162">Тестирование веб-части</span><span class="sxs-lookup"><span data-stu-id="01e00-162">Test your web part</span></span>

<span data-ttu-id="01e00-163">Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Для тестирования веб-частей, которые используют microsoft Graph набор средств, необходимо использовать веб-части с помощью веб-части с проверкой подлинности, так как для вызова Microsoft Graph компонентам необходим контекст проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="01e00-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="01e00-164">Вы можете найти свою уехавную работу по адресу **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx.**</span><span class="sxs-lookup"><span data-stu-id="01e00-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="01e00-165">Откройте файл в проекте и замените значение URL-адреса для `config\serve.json` `initialPage` вашей хост-области:</span><span class="sxs-lookup"><span data-stu-id="01e00-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="01e00-166">Сохраните файл и запустите следующую команду в консоли, чтобы создать и просмотреть веб-часть:</span><span class="sxs-lookup"><span data-stu-id="01e00-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="01e00-167">В браузере будет автоматически открыта ваша уеханая работа.</span><span class="sxs-lookup"><span data-stu-id="01e00-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="01e00-168">Добавьте веб-часть на страницу, и вы увидите ее с набор средств Microsoft Graph!</span><span class="sxs-lookup"><span data-stu-id="01e00-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="01e00-169">Если команда gulp serve по-прежнему работает в консоли, вы можете продолжать вносить изменения в код, а затем просто обновлять браузер, чтобы увидеть изменения.</span><span class="sxs-lookup"><span data-stu-id="01e00-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="01e00-170">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="01e00-170">Next Steps</span></span>
- <span data-ttu-id="01e00-171">Ознакомьтесь с этим пошаговом руководстве по [построению веб-части SharePoint.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)</span><span class="sxs-lookup"><span data-stu-id="01e00-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="01e00-172">Попробуйте компоненты в игровой [области.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="01e00-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="01e00-173">Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)</span><span class="sxs-lookup"><span data-stu-id="01e00-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="01e00-174">Сообщать об ошибках или оставлять запрос на функции на [GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="01e00-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>