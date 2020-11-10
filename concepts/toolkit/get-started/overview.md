---
title: Начало работы с набором средств Microsoft Graph
description: Приступите к работе с набором инструментов Microsoft Graph в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977137"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="169ee-103">Начало работы с набором средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="169ee-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="169ee-104">Компоненты набора инструментов Microsoft Graph легко можно добавить в веб-приложение, веб-часть SharePoint или вкладки Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="169ee-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="169ee-105">Компоненты основываются на веб-стандартах и могут использоваться как в простых проектах JavaScript, так и на популярных веб-платформах, таких как REACH, угловой, Vue.js и многое другое.</span><span class="sxs-lookup"><span data-stu-id="169ee-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="169ee-106">Вы можете посмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набором средств.</span><span class="sxs-lookup"><span data-stu-id="169ee-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="169ee-107">Настройка клиента Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="169ee-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="169ee-108">Для разработки с помощью набора инструментов вам необходим доступ к клиенту Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="169ee-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="169ee-109">Если у вас его нет, вы можете получить бесплатную подписку на Microsoft 365 для разработчиков, [присоединяясь к программе для разработчиков microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="169ee-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="169ee-110">Сведения о том, как настроить подписку, можно найти [в разделе Настройка подписки на Microsoft 365 для разработчиков](/office/developer-program/microsoft-365-developer-program-get-started).</span><span class="sxs-lookup"><span data-stu-id="169ee-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="169ee-111">Настройка среды разработки</span><span class="sxs-lookup"><span data-stu-id="169ee-111">Set up your development environment</span></span>
<span data-ttu-id="169ee-112">Для разработки с помощью набора инструментов вам потребуется текстовый редактор или IDE.</span><span class="sxs-lookup"><span data-stu-id="169ee-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="169ee-113">Вы можете использовать нужный редактор или IDE или установить и использовать [Visual Studio Code](https://code.visualstudio.com/download) бесплатно.</span><span class="sxs-lookup"><span data-stu-id="169ee-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="169ee-114">Кроме того, вам потребуется современный веб-браузер, например Microsoft EDGE, Google Chrome или Firefox.</span><span class="sxs-lookup"><span data-stu-id="169ee-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="169ee-115">Кроме того, вам потребуется LTS версия Node.js, которую можно установить из [NodeJS.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="169ee-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="169ee-116">Использование набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="169ee-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="169ee-117">Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="169ee-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="169ee-118">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="169ee-118">Use via mgt-loader</span></span>
<span data-ttu-id="169ee-119">Чтобы использовать набор средств с помощью элемента управления "центр управления", добавьте ссылку в скрипт в код:</span><span class="sxs-lookup"><span data-stu-id="169ee-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="169ee-120">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="169ee-120">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="169ee-121">Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения.</span><span class="sxs-lookup"><span data-stu-id="169ee-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="169ee-122">Чтобы использовать модули ES6, добавьте в проект пакет NPM:</span><span class="sxs-lookup"><span data-stu-id="169ee-122">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="169ee-123">Теперь вы можете ссылаться на все компоненты на странице, которые вы используете:</span><span class="sxs-lookup"><span data-stu-id="169ee-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="169ee-124">Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:</span><span class="sxs-lookup"><span data-stu-id="169ee-124">Or, just reference the component you need and avoid loading everything else:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a><span data-ttu-id="169ee-125">Polyfills</span><span class="sxs-lookup"><span data-stu-id="169ee-125">Polyfills</span></span>

<span data-ttu-id="169ee-126">Если вы используете модули ES6 из пакета NPM и используете [браузер, например IE11](https://caniuse.com/#search=components) , который не поддерживает встроенные веб-компоненты, необходимо включить в проект только те, которые не включены автоматически.</span><span class="sxs-lookup"><span data-stu-id="169ee-126">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="169ee-127">С помощью заполнения в браузерах можно заполнять отсутствующие возможности браузера в браузерах, которые по-прежнему находятся в процессе обновления для поддержки стандартов Вебккомпонент.</span><span class="sxs-lookup"><span data-stu-id="169ee-127">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support webcComponent standards.</span></span> <span data-ttu-id="169ee-128">Инструкции и дополнительные сведения [см.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="169ee-128">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="169ee-129">При использовании набора инструментов с помощью скрипта управления, в котором используется набор средств.</span><span class="sxs-lookup"><span data-stu-id="169ee-129">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="169ee-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="169ee-130">Next Steps</span></span>
<span data-ttu-id="169ee-131">Теперь вы готовы приступить к разработке с помощью набора инструментов Microsoft Graph!</span><span class="sxs-lookup"><span data-stu-id="169ee-131">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="169ee-132">Ниже приведены руководства, которые помогут вам приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="169ee-132">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="169ee-133">Создание приложения Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="169ee-133">Create an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="169ee-134">[Создание веб-приложения](./build-a-web-app.md) (Ванилла JavaScript)</span><span class="sxs-lookup"><span data-stu-id="169ee-134">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="169ee-135">Создание веб-части SharePoint</span><span class="sxs-lookup"><span data-stu-id="169ee-135">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="169ee-136">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="169ee-136">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="169ee-137">Использование набора инструментов с откликом</span><span class="sxs-lookup"><span data-stu-id="169ee-137">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="169ee-138">Использование набора инструментов с угловой</span><span class="sxs-lookup"><span data-stu-id="169ee-138">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
