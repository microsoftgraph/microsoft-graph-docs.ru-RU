---
title: Набор средств Microsoft Graph
description: Набор инструментов Microsoft Graph представляет собой набор ресуабле, независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2b8a7b3b93407410f31b17253f070065b6800b98
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275831"
---
# <a name="microsoft-graph-toolkit"></a><span data-ttu-id="bb849-103">Набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bb849-103">Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bb849-104">Набор инструментов Microsoft Graph представляет собой набор компонентов и вспомогательных программ для доступа к Microsoft Graph, не зависящего от платформы.</span><span class="sxs-lookup"><span data-stu-id="bb849-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="bb849-105">Все компоненты могут получать доступ к Microsoft Graph без необходимости настройки.</span><span class="sxs-lookup"><span data-stu-id="bb849-105">All components can access Microsoft Graph without any customization required.</span></span>

<span data-ttu-id="bb849-106">Набор инструментов Microsoft Graph — это отличный ресурс для всех разработчиков, которые стремятся к созданию веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, выполняющей вызовы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb849-106">The Microsoft Graph Toolkit is a great resource for any developer looking to create a web app, Microsoft Teams tab, or SharePoint web part that makes calls to Microsoft Graph.</span></span> <span data-ttu-id="bb849-107">Предоставляя компоненты пользовательского интерфейса, предназначенные для внешнего вида и работы с Microsoft 365, набор инструментов сокращает время и стоимость интеграции с платформой.</span><span class="sxs-lookup"><span data-stu-id="bb849-107">By providing UI components that are designed to look and feel like Microsoft 365 experiences, the Toolkit reduces your time and cost to integrate with the platform.</span></span> <span data-ttu-id="bb849-108">Все компоненты пользовательского интерфейса проходят проверку подлинности и получают доступ к данным из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb849-108">All the UI components authenticate with and access data from Microsoft Graph.</span></span> <span data-ttu-id="bb849-109">Компоненты полностью настраиваются с помощью CSS и шаблонов, поэтому вы можете соотнесение с уникальной фирменной символикой и управлять содержимым, отображаемым в компонентах.</span><span class="sxs-lookup"><span data-stu-id="bb849-109">The components are fully customizable using CSS and templating so you can match your unique branding and control the content displayed in the components.</span></span>

## <a name="get-started"></a><span data-ttu-id="bb849-110">Начало работы</span><span class="sxs-lookup"><span data-stu-id="bb849-110">Get started</span></span>

<span data-ttu-id="bb849-111">Вы можете использовать компоненты, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="bb849-111">You can use the components by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

![Начало работы](/images/get-started.gif)

<span data-ttu-id="bb849-113">Сведения о том, как приступить к работе с набором инструментов Microsoft Graph, можно найти в [видеоролике](https://www.youtube.com/watch?v=oZCGb2MMxa0)"Приступая к работе".</span><span class="sxs-lookup"><span data-stu-id="bb849-113">For details about how to get started with the Microsoft Graph Toolkit, see the [Get started video](https://www.youtube.com/watch?v=oZCGb2MMxa0).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="bb849-114">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="bb849-114">Use via mgt-loader</span></span>

<span data-ttu-id="bb849-115">Смотрите [Пример жсфиддле](https://jsfiddle.net/metulev/9phqxLd5/)фоловинг.</span><span class="sxs-lookup"><span data-stu-id="bb849-115">See the folowing [jsfiddle example](https://jsfiddle.net/metulev/9phqxLd5/).</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="bb849-116">Затем можно использовать компоненты на HTML-странице.</span><span class="sxs-lookup"><span data-stu-id="bb849-116">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="bb849-117">Ниже приведен полный рабочий пример с поставщиком MSAL.</span><span class="sxs-lookup"><span data-stu-id="bb849-117">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="bb849-118">**Примечание:** Для перенаправления проверки подлинности MSAL необходимо, чтобы страница была размещена на веб-сервере.</span><span class="sxs-lookup"><span data-stu-id="bb849-118">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="bb849-119">Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="bb849-119">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="bb849-120">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="bb849-120">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="bb849-121">С помощью модулей ES6 вы можете получить полный доступ к процессу объединения, и вы можете объединить только код, который требуется для вашего сайта.</span><span class="sxs-lookup"><span data-stu-id="bb849-121">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="bb849-122">Сначала добавьте пакет NPM:</span><span class="sxs-lookup"><span data-stu-id="bb849-122">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="bb849-123">Теперь вы можете ссылаться на все компоненты на странице, которую вы используете:</span><span class="sxs-lookup"><span data-stu-id="bb849-123">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="bb849-124">Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:</span><span class="sxs-lookup"><span data-stu-id="bb849-124">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="bb849-125">Аналогичным образом, чтобы добавить поставщика, можно добавить его в качестве компонента:</span><span class="sxs-lookup"><span data-stu-id="bb849-125">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="bb849-126">или добавьте его в код:</span><span class="sxs-lookup"><span data-stu-id="bb849-126">or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="bb849-127">Доступа</span><span class="sxs-lookup"><span data-stu-id="bb849-127">Providers</span></span>

<span data-ttu-id="bb849-128">Компоненты лучше всего подходят для использования с [поставщиками](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="bb849-128">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="bb849-129">Поставщик предоставляет доступ к проверке подлинности и интерфейсам API, которые используются компонентами для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb849-129">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="bb849-130">Набор средств содержит поставщики для [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md)и надстроек Office (ожидается в ближайшее время).</span><span class="sxs-lookup"><span data-stu-id="bb849-130">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md), and Office Add-ins (coming soon).</span></span> <span data-ttu-id="bb849-131">Вы также можете создавать собственные поставщики, расширяя абстрактный класс [Ипровидер].</span><span class="sxs-lookup"><span data-stu-id="bb849-131">You can also create your own providers by extending the [IProvider] abstract class.</span></span>

## <a name="polyfills"></a><span data-ttu-id="bb849-132">Polyfills</span><span class="sxs-lookup"><span data-stu-id="bb849-132">Polyfills</span></span>

<span data-ttu-id="bb849-133">Если вы используете модули ES6 из пакета NPM, не забудьте включить в проект только те, которые не включены автоматически.</span><span class="sxs-lookup"><span data-stu-id="bb849-133">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="bb849-134">Дополнительные сведения [см.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="bb849-134">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="bb849-135">Если вы используете скрипт МГТ-лоадер. js из пакета в унпкг, то эти функции уже включены.</span><span class="sxs-lookup"><span data-stu-id="bb849-135">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="bb849-136">Использование компонентов с реагирует, радиально и другими платформами</span><span class="sxs-lookup"><span data-stu-id="bb849-136">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="bb849-137">Веб-компоненты основываются на нескольких веб-стандартах и могут использоваться с любой уже используемой платформой.</span><span class="sxs-lookup"><span data-stu-id="bb849-137">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="bb849-138">Однако не все платформы обрабатывают веб-компоненты одинаковым образом.</span><span class="sxs-lookup"><span data-stu-id="bb849-138">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="bb849-139">Чтобы узнать больше о возможностях, которые могут применяться в зависимости от вашей платформы, ознакомьтесь со статьей " [настраиваемые элементы везде](https://custom-elements-everywhere.com/) ".</span><span class="sxs-lookup"><span data-stu-id="bb849-139">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="bb849-140">В следующих разделах приводится краткий обзор использования компонентов набора инструментов Microsoft Graph с откликом и радиальным.</span><span class="sxs-lookup"><span data-stu-id="bb849-140">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="bb849-141">React</span><span class="sxs-lookup"><span data-stu-id="bb849-141">React</span></span>

<span data-ttu-id="bb849-142">Реагирует, что все данные передаются в настраиваемые элементы формы HTML Attributes.</span><span class="sxs-lookup"><span data-stu-id="bb849-142">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="bb849-143">Для примитивных данных это нормально, но не работает при передаче форматированных данных, таких как объекты или массивы.</span><span class="sxs-lookup"><span data-stu-id="bb849-143">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="bb849-144">В этих случаях для передачи объекта потребуется использовать `ref` объект.</span><span class="sxs-lookup"><span data-stu-id="bb849-144">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="bb849-145">Пример</span><span class="sxs-lookup"><span data-stu-id="bb849-145">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="bb849-146">Так как реакция реализует собственную виртуальную систему обработки событий, она не может прослушивать события модели DOM, поступающие из настраиваемых элементов, без использования обходного пути.</span><span class="sxs-lookup"><span data-stu-id="bb849-146">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="bb849-147">Необходимо использовать элемент a `ref` для ссылки на компоненты набора инструментов и вручную присоединить прослушиватели событий с помощью метода addEventListener, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="bb849-147">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

```jsx
// you can just import a single component
import '@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js';

class App extends Component {
  render() {
    return <mgt-login ref="loginComponent" />;
  }

  componentDidMount() {
    this.refs.loginComponent.addEventListener('loginCompleted', e => {
      // handle event
    });
  }
}
```

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="bb849-148">Реакция, typescript и целевой серверу</span><span class="sxs-lookup"><span data-stu-id="bb849-148">React, Typescript, and TSX</span></span>

<span data-ttu-id="bb849-149">Известная ошибка может возникать при использовании настраиваемых элементов с помощью реакции и typescript.</span><span class="sxs-lookup"><span data-stu-id="bb849-149">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="bb849-150">Typescript выдаст ошибку при попытке использовать компонент в целевом элементе.</span><span class="sxs-lookup"><span data-stu-id="bb849-150">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="bb849-151">Временное решение заключается в определении настраиваемого элемента в коде, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="bb849-151">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="bb849-152">Затем вы можете использовать его в целевом параметре как `<mgt-login></mgt-login>`.</span><span class="sxs-lookup"><span data-stu-id="bb849-152">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="bb849-153">Angular</span><span class="sxs-lookup"><span data-stu-id="bb849-153">Angular</span></span>

<span data-ttu-id="bb849-154">Синтаксис привязки по умолчанию в радиальной системе всегда будет задавайте свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="bb849-154">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="bb849-155">Это хорошо подходит для сложных данных, таких как объекты и массивы, а также для примитивных значений.</span><span class="sxs-lookup"><span data-stu-id="bb849-155">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="bb849-156">Прежде чем использовать настраиваемые элементы, включите в него `app.module.ts` `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator`настраиваемые элементы, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="bb849-156">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

<span data-ttu-id="bb849-157">Затем вы можете импортировать компонент, который вы хотите использовать, в файле Component \*. TS.</span><span class="sxs-lookup"><span data-stu-id="bb849-157">You can then import the component you'd like to use in your component \*.ts file.</span></span>

```ts
import { Component } from '@angular/core';
import '@microsoft/mgt/dist/es6/components/mgt-person/mgt-person';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  person = {
    displayName: 'Nikola Metulev'
  };
}
```

<span data-ttu-id="bb849-158">Наконец, используйте компонент, как обычно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="bb849-158">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
