---
title: Создайте SharePoint веб-часть с помощью microsoft Graph набор средств
description: Начало работы с помощью веб-Graph набор средств майкрософт для создания SharePoint веб-части.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c1f4be864c9e762e164980bc20abb4195df5c9f7
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629135"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="0728d-103">Создайте SharePoint веб-часть с помощью microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="0728d-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0728d-104">В этом разделе описывается использование компонентов Microsoft Graph набор средств в SharePoint [клиентской веб-части](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span><span class="sxs-lookup"><span data-stu-id="0728d-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="0728d-105">Начало работы включает в себя следующие действия:</span><span class="sxs-lookup"><span data-stu-id="0728d-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="0728d-106">Настройка среды разработки и создание веб-части.</span><span class="sxs-lookup"><span data-stu-id="0728d-106">Set up your development environment and create a web part.</span></span>
1. <span data-ttu-id="0728d-107">Добавьте пакет Microsoft Graph набор средств SharePoint Framework.</span><span class="sxs-lookup"><span data-stu-id="0728d-107">Add the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="0728d-108">Добавьте SharePoint поставщика.</span><span class="sxs-lookup"><span data-stu-id="0728d-108">Add the SharePoint Provider.</span></span>
1. <span data-ttu-id="0728d-109">Добавление компонентов.</span><span class="sxs-lookup"><span data-stu-id="0728d-109">Add components.</span></span>
1. <span data-ttu-id="0728d-110">Настройка разрешений.</span><span class="sxs-lookup"><span data-stu-id="0728d-110">Configure permissions.</span></span>
1. <span data-ttu-id="0728d-111">Развертывание пакета microsoft Graph набор средств SharePoint Framework.</span><span class="sxs-lookup"><span data-stu-id="0728d-111">Deploy the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="0728d-112">Сборка и развертывание веб-части.</span><span class="sxs-lookup"><span data-stu-id="0728d-112">Build and deploy your web part.</span></span>
1. <span data-ttu-id="0728d-113">Проверьте веб-часть.</span><span class="sxs-lookup"><span data-stu-id="0728d-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="0728d-114">Настройка среды SharePoint Framework разработки и создание новой веб-части</span><span class="sxs-lookup"><span data-stu-id="0728d-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="0728d-115">Выполните действия по [настройкам среды SharePoint Framework разработки,](/sharepoint/dev/spfx/set-up-your-development-environment) а затем [создайте новую веб-часть.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)</span><span class="sxs-lookup"><span data-stu-id="0728d-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="0728d-116">Добавление пакета microsoft Graph набор средств SharePoint Framework</span><span class="sxs-lookup"><span data-stu-id="0728d-116">Add the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="0728d-117">Чтобы не допустить SharePoint Framework компонентов Microsoft Graph набор средств на странице, необходимо развернуть пакет Microsoft Graph набор средств SharePoint Framework для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этого пакета.</span><span class="sxs-lookup"><span data-stu-id="0728d-117">To prevent multiple SharePoint Framework components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this package.</span></span>

<span data-ttu-id="0728d-118">Пакет Microsoft Graph набор средств SharePoint Framework содержит библиотеку SharePoint Framework, которая регистрирует один экземпляр компонентов Microsoft Graph набор средств в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0728d-118">The Microsoft Graph Toolkit SharePoint Framework package contains a SharePoint Framework library that registers a single instance of Microsoft Graph Toolkit components in SharePoint.</span></span>

<span data-ttu-id="0728d-119">Установите пакет microsoft Graph набор средств SharePoint Framework npm с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="0728d-119">Install the Microsoft Graph Toolkit SharePoint Framework npm package using the following command:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="0728d-120">Добавление SharePoint поставщика</span><span class="sxs-lookup"><span data-stu-id="0728d-120">Add the SharePoint Provider</span></span>

<span data-ttu-id="0728d-121">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="0728d-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="0728d-122">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="0728d-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="0728d-123">SharePoint веб-части всегда существуют в контексте проверки подлинности, так как пользователю уже пришлось войти, чтобы попасть на страницу, на которую размещена ваша веб-часть.</span><span class="sxs-lookup"><span data-stu-id="0728d-123">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="0728d-124">Используйте этот контекст для инициализации [SharePoint поставщика](../providers/sharepoint.md).</span><span class="sxs-lookup"><span data-stu-id="0728d-124">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="0728d-125">Сначала добавьте поставщика в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="0728d-125">First, add the provider to your web part.</span></span> <span data-ttu-id="0728d-126">Найдите файл в папке проекта и добавьте следующую строку в верхнюю часть файла прямо под `src\webparts\<your-project>\<your-web-part>.ts` `import` существующими утверждениями:</span><span class="sxs-lookup"><span data-stu-id="0728d-126">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

<span data-ttu-id="0728d-127">Далее необходимо инициализировать поставщика с помощью контекста проверки подлинности в `onInit()` методе веб-части.</span><span class="sxs-lookup"><span data-stu-id="0728d-127">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="0728d-128">В том же файле добавьте следующий код прямо перед `public render(): void {` строкой:</span><span class="sxs-lookup"><span data-stu-id="0728d-128">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a><span data-ttu-id="0728d-129">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="0728d-129">Add components</span></span>

<span data-ttu-id="0728d-130">Теперь можно приступить к добавлению компонентов в веб-часть.</span><span class="sxs-lookup"><span data-stu-id="0728d-130">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="0728d-131">Просто добавьте компоненты в HTML внутри метода, и компоненты будут использовать контекст SharePoint для доступа к `render()` Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0728d-131">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="0728d-132">Например, чтобы добавить компонент [Person,](../components/person.md)код будет выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="0728d-132">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> <span data-ttu-id="0728d-133">Если вы строите веб-часть с React, см. в [@microsoft/mgt-spfx документы,](./mgt-spfx.md#react) чтобы узнать, как использовать `@microsoft/mgt-react` .</span><span class="sxs-lookup"><span data-stu-id="0728d-133">If you're building a web part using React, see the [@microsoft/mgt-spfx docs](./mgt-spfx.md#react) to learn how to use `@microsoft/mgt-react`.</span></span>

## <a name="configure-permissions"></a><span data-ttu-id="0728d-134">Настройка разрешений</span><span class="sxs-lookup"><span data-stu-id="0728d-134">Configure permissions</span></span>

<span data-ttu-id="0728d-135">Чтобы вызвать microsoft Graph из SharePoint Framework приложения, необходимо запросить необходимые разрешения в пакете решений, а администратору Microsoft 365 необходимо утвердить запрашиваемую разрешения.</span><span class="sxs-lookup"><span data-stu-id="0728d-135">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="0728d-136">Чтобы добавить разрешения в пакет решений, найдите и откройте `config\package-solution.json` файл и установите:</span><span class="sxs-lookup"><span data-stu-id="0728d-136">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="0728d-137">Чуть ниже этой строки добавьте следующее:</span><span class="sxs-lookup"><span data-stu-id="0728d-137">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="0728d-138">Определите Graph разрешения API Майкрософт в зависимости от компонентов, которые вы используете.</span><span class="sxs-lookup"><span data-stu-id="0728d-138">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="0728d-139">На странице документации каждого компонента содержится список разрешений, которые необходимы компоненту.</span><span class="sxs-lookup"><span data-stu-id="0728d-139">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="0728d-140">Вам потребуется добавить каждое разрешение, необходимое `webApiPermissionRequests` для .</span><span class="sxs-lookup"><span data-stu-id="0728d-140">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="0728d-141">Например, если вы используете компонент Person и компонент Agenda, вы можете `webApiPermissionRequests` выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="0728d-141">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="0728d-142">Развертывание пакета microsoft Graph набор средств SharePoint Framework</span><span class="sxs-lookup"><span data-stu-id="0728d-142">Deploy the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="0728d-143">Перед развертывание SharePoint Framework пакета для клиента необходимо развернуть пакет Microsoft Graph набор средств SharePoint Framework для клиента.</span><span class="sxs-lookup"><span data-stu-id="0728d-143">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="0728d-144">Вы можете скачать пакет, соответствующий версии microsoft Graph набор средств, используемой в [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) проекте, из раздела Выпуски на GitHub.</span><span class="sxs-lookup"><span data-stu-id="0728d-144">You can download the package corresponding to the version of Microsoft Graph Toolkit that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="0728d-145">Поскольку в клиенте SharePoint Framework может быть установлена только одна версия библиотеки Graph набор средств Microsoft, прежде чем использовать microsoft Graph набор средств в решении, определите, имеет ли ваша организация или клиент уже развернута версия библиотеки SharePoint Framework и использовать ту же версию.</span><span class="sxs-lookup"><span data-stu-id="0728d-145">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

<span data-ttu-id="0728d-146">Загрузив пакет Microsoft Graph набор средств SharePoint Framework sppkg, загрузите его в каталог SharePoint приложения.</span><span class="sxs-lookup"><span data-stu-id="0728d-146">After downloading the Microsoft Graph Toolkit SharePoint Framework .sppkg package, upload it to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="0728d-147">Перейдите на [страницу Дополнительные функции центра администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="0728d-147">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="0728d-148">Выберите **Открыть** в **приложениях,** а затем нажмите **каталог приложений** и **раздать** приложения для SharePoint .</span><span class="sxs-lookup"><span data-stu-id="0728d-148">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="0728d-149">Upload `.sppkg` файл и нажмите кнопку **Развертывание.**</span><span class="sxs-lookup"><span data-stu-id="0728d-149">Upload your `.sppkg` file, and click **Deploy**.</span></span>

## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="0728d-150">Сборка и развертывание веб-части</span><span class="sxs-lookup"><span data-stu-id="0728d-150">Build and deploy your web part</span></span>

<span data-ttu-id="0728d-151">Теперь вы создайте приложение и разверните его в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0728d-151">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="0728d-152">Создайте приложение, запуская следующие команды:</span><span class="sxs-lookup"><span data-stu-id="0728d-152">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="0728d-153">В `sharepoint/solution` папке будет новый `.sppkg` файл.</span><span class="sxs-lookup"><span data-stu-id="0728d-153">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="0728d-154">Вам потребуется загрузить этот файл в SharePoint каталога приложений в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0728d-154">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="0728d-155">Перейдите на [страницу Дополнительные функции центра администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="0728d-155">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="0728d-156">Выберите **Открыть** в **приложениях,** а затем нажмите **каталог приложений** и **раздать** приложения для SharePoint .</span><span class="sxs-lookup"><span data-stu-id="0728d-156">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="0728d-157">Upload `.sppkg` файл и нажмите кнопку **Развертывание.**</span><span class="sxs-lookup"><span data-stu-id="0728d-157">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="0728d-158">Далее необходимо утвердить разрешения в качестве администратора.</span><span class="sxs-lookup"><span data-stu-id="0728d-158">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="0728d-159">Перейдите в **центр SharePoint администрирования.**</span><span class="sxs-lookup"><span data-stu-id="0728d-159">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="0728d-160">В левой навигации выберите **Расширенный** и затем **API Access**.</span><span class="sxs-lookup"><span data-stu-id="0728d-160">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="0728d-161">Вы должны видеть ожидающих запросов для каждого из разрешений, добавленных в `config\package-solution.json` файл.</span><span class="sxs-lookup"><span data-stu-id="0728d-161">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="0728d-162">Выберите и утвердим каждое разрешение.</span><span class="sxs-lookup"><span data-stu-id="0728d-162">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="0728d-163">Проверка веб-части</span><span class="sxs-lookup"><span data-stu-id="0728d-163">Test your web part</span></span>

<span data-ttu-id="0728d-164">Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Чтобы протестировать веб-части, которые используют microsoft Graph набор средств, необходимо использовать упорядоченный контекст, чтобы вызвать microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0728d-164">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="0728d-165">Вы можете найти у себя на сайте **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx.**</span><span class="sxs-lookup"><span data-stu-id="0728d-165">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="0728d-166">Откройте файл в проекте и замените значение URL-адресом для `config\serve.json` `initialPage` принимающей работы:</span><span class="sxs-lookup"><span data-stu-id="0728d-166">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="0728d-167">Сохраните файл и запустите следующую команду в консоли для создания и предварительного просмотра веб-части:</span><span class="sxs-lookup"><span data-stu-id="0728d-167">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="0728d-168">В браузере автоматически откроется хост-хозяйная работа.</span><span class="sxs-lookup"><span data-stu-id="0728d-168">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="0728d-169">Добавьте веб-часть на страницу, и вы увидите веб-часть с компонентами Microsoft Graph набор средств в действии!</span><span class="sxs-lookup"><span data-stu-id="0728d-169">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="0728d-170">До тех пор, пока команда службы глоток продолжает работать в консоли, вы можете продолжать вносить изменения в код, а затем просто обновить браузер, чтобы увидеть изменения.</span><span class="sxs-lookup"><span data-stu-id="0728d-170">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0728d-171">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0728d-171">Next Steps</span></span>
- <span data-ttu-id="0728d-172">Ознакомьтесь с этим пошаговом руководстве по SharePoint [веб-части.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)</span><span class="sxs-lookup"><span data-stu-id="0728d-172">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="0728d-173">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="0728d-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="0728d-174">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="0728d-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="0728d-175">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="0728d-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
