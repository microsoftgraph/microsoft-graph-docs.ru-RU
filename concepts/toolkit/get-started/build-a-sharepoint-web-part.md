---
title: Создание веб-части SharePoint с помощью набора инструментов Microsoft Graph
description: Приступите к работе с набором инструментов Microsoft Graph для создания веб-части SharePoint.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: b2ae71a8fb37e088c0497716fdf4d1cdc42f41ef
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288530"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="03433-103">Создание веб-части SharePoint с помощью набора инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="03433-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="03433-104">В этом разделе описывается, как использовать компоненты набора инструментов Microsoft Graph в [клиентской веб-части SharePoint](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span><span class="sxs-lookup"><span data-stu-id="03433-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="03433-105">Приступая к работе состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="03433-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="03433-106">Настройте среду разработки и создайте веб-часть.</span><span class="sxs-lookup"><span data-stu-id="03433-106">Set up your development environment and create a web part.</span></span>
2. <span data-ttu-id="03433-107">Обновление TypeScript в проекте.</span><span class="sxs-lookup"><span data-stu-id="03433-107">Update TypeScript in your project.</span></span>
3. <span data-ttu-id="03433-108">Добавьте набор инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="03433-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="03433-109">Добавьте поставщика SharePoint.</span><span class="sxs-lookup"><span data-stu-id="03433-109">Add the SharePoint Provider.</span></span>
5. <span data-ttu-id="03433-110">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="03433-110">Add components.</span></span>
6. <span data-ttu-id="03433-111">Настройка разрешений.</span><span class="sxs-lookup"><span data-stu-id="03433-111">Configure permissions.</span></span>
7. <span data-ttu-id="03433-112">Создание и развертывание веб-части.</span><span class="sxs-lookup"><span data-stu-id="03433-112">Build and deploy your web part.</span></span>
8. <span data-ttu-id="03433-113">Протестируйте веб-часть.</span><span class="sxs-lookup"><span data-stu-id="03433-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="03433-114">Настройка среды разработки SharePoint Framework и создание новой веб-части</span><span class="sxs-lookup"><span data-stu-id="03433-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="03433-115">Выполните действия, чтобы [настроить среду разработки SharePoint Framework](/sharepoint/dev/spfx/set-up-your-development-environment) , а затем [Создайте новую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="03433-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="update-typescript-in-your-project"></a><span data-ttu-id="03433-116">Обновление TypeScript в проекте</span><span class="sxs-lookup"><span data-stu-id="03433-116">Update TypeScript in your project</span></span>

<span data-ttu-id="03433-117">Набор средств Microsoft Graph требует typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="03433-117">The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="03433-118">Перед добавлением набора средств в проект убедитесь, что вы используете [поддерживаемую версию typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="03433-118">Before adding the Toolkit to your project, make sure you're using a [supported version of Typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span> <span data-ttu-id="03433-119">Например, чтобы добавить typescript 3,7, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="03433-119">For example, to add Typescript 3.7, use the following command:</span></span>

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
<span data-ttu-id="03433-120">Затем найдите `tsconfig.json` файл в папке проекта, откройте файл и найдите следующую строку:</span><span class="sxs-lookup"><span data-stu-id="03433-120">Then, locate the `tsconfig.json` file in your project folder, open the file, and look for this line:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
<span data-ttu-id="03433-121">Замените строку следующим:</span><span class="sxs-lookup"><span data-stu-id="03433-121">Replace the line with:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="03433-122">Добавление набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="03433-122">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="03433-123">Установите пакет инструментов набора инструментов Microsoft Graph NPM и с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="03433-123">Install the Microsoft Graph Toolkit npm package and polyfills with the following command:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="03433-124">Если вы планируете поддерживать IE11 в веб-частях, вам потребуется выполнить дополнительные действия, чтобы обеспечить совместимость между браузерами:</span><span class="sxs-lookup"><span data-stu-id="03433-124">If you plan to support IE11 in your web parts, you'll need to follow additional steps to ensure cross-browser compatibility:</span></span>

1. <span data-ttu-id="03433-125">Установите следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="03433-125">Install the following packages:</span></span>
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. <span data-ttu-id="03433-126">Добавьте следующий код в следующий код `gulpfile.js` `build.initialize(gulp)` :</span><span class="sxs-lookup"><span data-stu-id="03433-126">Add the following code to `gulpfile.js`, right above `build.initialize(gulp)`:</span></span>
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
3. <span data-ttu-id="03433-127">В `src\webparts\<your-project>\<your-web-part>.ts` файле импортируйте указанные ниже операции с помощью оператора заполнил перед поставщиком SharePoint на следующем этапе.</span><span class="sxs-lookup"><span data-stu-id="03433-127">In your `src\webparts\<your-project>\<your-web-part>.ts` file, import the following polyfills before the SharePoint provider in the next step.</span></span>

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

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="03433-128">Добавление поставщика SharePoint</span><span class="sxs-lookup"><span data-stu-id="03433-128">Add the SharePoint Provider</span></span>

<span data-ttu-id="03433-129">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="03433-129">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="03433-130">Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="03433-130">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="03433-131">Веб-части SharePoint всегда существуют в контексте, прошедшем проверку подлинности, так как пользователь уже выполнил вход, чтобы перейти на страницу, на которой размещается веб-часть.</span><span class="sxs-lookup"><span data-stu-id="03433-131">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="03433-132">Используйте этот контекст для инициализации [поставщика SharePoint](../providers/sharepoint.md).</span><span class="sxs-lookup"><span data-stu-id="03433-132">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="03433-133">Сначала добавьте поставщик в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="03433-133">First, add the provider to your web part.</span></span> <span data-ttu-id="03433-134">Выберите `src\webparts\<your-project>\<your-web-part>.ts` файл в папке проекта и добавьте следующую строку в верхнюю часть файла, расположенную ниже существующих `import` операторов:</span><span class="sxs-lookup"><span data-stu-id="03433-134">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

<span data-ttu-id="03433-135">Далее необходимо инициализировать поставщика с помощью контекста, прошедшего проверку подлинности, в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="03433-135">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="03433-136">В том же файле добавьте следующий код перед `public render(): void {` строкой:</span><span class="sxs-lookup"><span data-stu-id="03433-136">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a><span data-ttu-id="03433-137">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="03433-137">Add components</span></span>

<span data-ttu-id="03433-138">Теперь можно приступить к добавлению компонентов в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="03433-138">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="03433-139">Просто добавьте компоненты в HTML-код в `render()` методе, и компоненты будут использовать контекст SharePoint для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="03433-139">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="03433-140">Например, чтобы добавить [компонент Person](../components/person.md), ваш код будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="03433-140">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="03433-141">Настройка разрешений</span><span class="sxs-lookup"><span data-stu-id="03433-141">Configure permissions</span></span>

<span data-ttu-id="03433-142">Для вызова Microsoft Graph из приложения SharePoint Framework необходимо запросить необходимые разрешения в пакете решения, а администратор клиента Microsoft 365 — утвердить запрошенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="03433-142">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="03433-143">Чтобы добавить разрешения в пакет решения, перейдите к файлу и откройте его `config\package-solution.json` и задайте следующие настройки:</span><span class="sxs-lookup"><span data-stu-id="03433-143">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="03433-144">Под этой строкой добавьте следующий код:</span><span class="sxs-lookup"><span data-stu-id="03433-144">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="03433-145">Определите, какие разрешения API Microsoft Graph необходимы в зависимости от используемых компонентов.</span><span class="sxs-lookup"><span data-stu-id="03433-145">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="03433-146">На странице документации каждого компонента представлен список разрешений, которые требуются компоненту.</span><span class="sxs-lookup"><span data-stu-id="03433-146">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="03433-147">Вам потребуется добавить каждое разрешение, необходимое для `webApiPermissionRequests` .</span><span class="sxs-lookup"><span data-stu-id="03433-147">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="03433-148">Например, если вы используете компонент Person и компонент повестки, он `webApiPermissionRequests` может выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="03433-148">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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
## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="03433-149">Построение и развертывание веб-части</span><span class="sxs-lookup"><span data-stu-id="03433-149">Build and deploy your web part</span></span>

<span data-ttu-id="03433-150">Теперь предстоит создать приложение и развернуть его в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="03433-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="03433-151">Постройте приложение, выполнив следующие команды:</span><span class="sxs-lookup"><span data-stu-id="03433-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="03433-152">В `sharepoint/solution` папке будет создан новый `.sppkg` файл.</span><span class="sxs-lookup"><span data-stu-id="03433-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="03433-153">Вам потребуется загрузить этот файл в каталог приложений SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="03433-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="03433-154">Перейдите на [страницу дополнительные компоненты своего центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span><span class="sxs-lookup"><span data-stu-id="03433-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="03433-155">Выберите пункт **Открыть** в разделе **приложения**, а затем выберите **Каталог приложений**и **Распространите приложения для SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="03433-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="03433-156">Отправьте `.sppkg` файл и нажмите кнопку **развернуть**.</span><span class="sxs-lookup"><span data-stu-id="03433-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="03433-157">Далее необходимо утвердить разрешения как администратор.</span><span class="sxs-lookup"><span data-stu-id="03433-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="03433-158">Перейдите в **центр администрирования SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="03433-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="03433-159">В левой области навигации выберите **Дополнительно** , а затем — **доступ к API**.</span><span class="sxs-lookup"><span data-stu-id="03433-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="03433-160">Для каждого разрешения, добавленного в файл, должны отображаться ожидающие запросы `config\package-solution.json` .</span><span class="sxs-lookup"><span data-stu-id="03433-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="03433-161">Выберите и утвердите каждое разрешение.</span><span class="sxs-lookup"><span data-stu-id="03433-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="03433-162">Тестирование веб-части</span><span class="sxs-lookup"><span data-stu-id="03433-162">Test your web part</span></span>

<span data-ttu-id="03433-163">Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Для тестирования веб-частей, использующих набор инструментов Microsoft Graph, необходимо использовать размещенную рабочую среду, так как для вызова Microsoft Graph необходимо, чтобы для компонентов подлинность контекста была подлинной.</span><span class="sxs-lookup"><span data-stu-id="03433-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="03433-164">Размещенный Workbench можно найти на сайте **https://<YOUR_TENANT>. SharePoint.com/_layouts/15/Workbench.aspx**.</span><span class="sxs-lookup"><span data-stu-id="03433-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="03433-165">Откройте `config\serve.json` файл в проекте и замените значение на `initialPage` URL-адрес размещенной рабочей области:</span><span class="sxs-lookup"><span data-stu-id="03433-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="03433-166">Сохраните файл, а затем выполните приведенную ниже команду в консоли, чтобы создать и просмотреть веб-часть:</span><span class="sxs-lookup"><span data-stu-id="03433-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="03433-167">Размещенная среда будет автоматически открываться в браузере.</span><span class="sxs-lookup"><span data-stu-id="03433-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="03433-168">Добавьте веб-часть на страницу, и вы должны увидеть веб-часть с компонентами набора инструментов Microsoft Graph в действии!</span><span class="sxs-lookup"><span data-stu-id="03433-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="03433-169">Пока команда gulp обслуживает все еще работает в консоли, вы можете продолжить внесение изменений в код, а затем просто обновить браузер, чтобы увидеть внесенные изменения.</span><span class="sxs-lookup"><span data-stu-id="03433-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="03433-170">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="03433-170">Next Steps</span></span>
- <span data-ttu-id="03433-171">Ознакомьтесь с пошаговыми руководствами по [созданию веб-части SharePoint](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span><span class="sxs-lookup"><span data-stu-id="03433-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="03433-172">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="03433-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="03433-173">Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="03433-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="03433-174">Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="03433-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>