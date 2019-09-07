---
title: Набор средств Microsoft Graph (Предварительная версия)
description: Набор средств Microsoft Graph — это набор независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4509e382b89dcd9c403695df2ff7d99115a7f8b4
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792865"
---
# <a name="microsoft-graph-toolkit-preview"></a><span data-ttu-id="31652-103">Набор средств Microsoft Graph (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="31652-103">Microsoft Graph Toolkit (preview)</span></span>

<span data-ttu-id="31652-104">Набор средств Microsoft Graph — это набор независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.</span><span class="sxs-lookup"><span data-stu-id="31652-104">The Microsoft Graph Toolkit is a collection of framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="31652-105">Все компоненты могут получать доступ к Microsoft Graph без необходимости настройки.</span><span class="sxs-lookup"><span data-stu-id="31652-105">All components can access Microsoft Graph without any customization required.</span></span>

>[!NOTE]
><span data-ttu-id="31652-106">Эта библиотека находится в предварительной версии и предназначена для более ранней разработки.</span><span class="sxs-lookup"><span data-stu-id="31652-106">This library is in preview and is in early development.</span></span> <span data-ttu-id="31652-107">Мы планируем вносить изменения и улучшения для всех компонентов и интерфейсов API на основе отзывов сообщества.</span><span class="sxs-lookup"><span data-stu-id="31652-107">We expect to make changes and improvements to all components and APIs based on feedback from the community.</span></span>

## <a name="get-started"></a><span data-ttu-id="31652-108">Начало работы</span><span class="sxs-lookup"><span data-stu-id="31652-108">Get started</span></span>

<span data-ttu-id="31652-109">Вы можете использовать компоненты, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="31652-109">You can use the components by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

<span data-ttu-id="31652-110">Сведения о том, как приступить к работе с набором инструментов Microsoft Graph, можно найти в [видеоролике](https://www.youtube.com/watch?v=oZCGb2MMxa0)"Приступая к работе".</span><span class="sxs-lookup"><span data-stu-id="31652-110">For details about how to get started with the Microsoft Graph Toolkit, see the [Get started video](https://www.youtube.com/watch?v=oZCGb2MMxa0).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="31652-111">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="31652-111">Use via mgt-loader</span></span>

<span data-ttu-id="31652-112">Смотрите [Пример жсфиддле](https://jsfiddle.net/metulev/9phqxLd5/)фоловинг.</span><span class="sxs-lookup"><span data-stu-id="31652-112">See the folowing [jsfiddle example](https://jsfiddle.net/metulev/9phqxLd5/).</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="31652-113">Затем можно использовать компоненты на HTML-странице.</span><span class="sxs-lookup"><span data-stu-id="31652-113">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="31652-114">Ниже приведен полный рабочий пример с поставщиком MSAL.</span><span class="sxs-lookup"><span data-stu-id="31652-114">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="31652-115">**Примечание:** Для перенаправления проверки подлинности MSAL необходимо, чтобы страница была размещена на веб-сервере.</span><span class="sxs-lookup"><span data-stu-id="31652-115">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="31652-116">Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="31652-116">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="31652-117">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="31652-117">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="31652-118">С помощью модулей ES6 вы можете получить полный доступ к процессу объединения, и вы можете объединить только код, который требуется для вашего сайта.</span><span class="sxs-lookup"><span data-stu-id="31652-118">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="31652-119">Сначала добавьте пакет NPM:</span><span class="sxs-lookup"><span data-stu-id="31652-119">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="31652-120">Теперь вы можете ссылаться на все компоненты на странице, которую вы используете:</span><span class="sxs-lookup"><span data-stu-id="31652-120">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="31652-121">Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:</span><span class="sxs-lookup"><span data-stu-id="31652-121">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="31652-122">Аналогичным образом, чтобы добавить поставщика, можно добавить его в качестве компонента:</span><span class="sxs-lookup"><span data-stu-id="31652-122">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="31652-123">или добавьте его в код:</span><span class="sxs-lookup"><span data-stu-id="31652-123">or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="31652-124">Доступа</span><span class="sxs-lookup"><span data-stu-id="31652-124">Providers</span></span>

<span data-ttu-id="31652-125">Компоненты лучше всего подходят для использования с [поставщиками](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="31652-125">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="31652-126">Поставщик предоставляет доступ к проверке подлинности и интерфейсам API, которые используются компонентами для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="31652-126">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="31652-127">Набор средств содержит поставщики для [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md)и надстроек Office (ожидается в ближайшее время).</span><span class="sxs-lookup"><span data-stu-id="31652-127">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md), and Office Add-ins (coming soon).</span></span> <span data-ttu-id="31652-128">Вы также можете создавать собственные поставщики, расширяя абстрактный класс [Ипровидер].</span><span class="sxs-lookup"><span data-stu-id="31652-128">You can also create your own providers by extending the [IProvider] abstract class.</span></span>

## <a name="polyfills"></a><span data-ttu-id="31652-129">Polyfills</span><span class="sxs-lookup"><span data-stu-id="31652-129">Polyfills</span></span>

<span data-ttu-id="31652-130">Если вы используете модули ES6 из пакета NPM, не забудьте включить в проект только те, которые не включены автоматически.</span><span class="sxs-lookup"><span data-stu-id="31652-130">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="31652-131">Дополнительные сведения [см.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="31652-131">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="31652-132">Если вы используете скрипт МГТ-лоадер. js из пакета в унпкг, то эти функции уже включены.</span><span class="sxs-lookup"><span data-stu-id="31652-132">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="31652-133">Использование компонентов с реагирует, радиально и другими платформами</span><span class="sxs-lookup"><span data-stu-id="31652-133">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="31652-134">Веб-компоненты основываются на нескольких веб-стандартах и могут использоваться с любой уже используемой платформой.</span><span class="sxs-lookup"><span data-stu-id="31652-134">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="31652-135">Однако не все платформы обрабатывают веб-компоненты одинаковым образом.</span><span class="sxs-lookup"><span data-stu-id="31652-135">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="31652-136">Чтобы узнать больше о возможностях, которые могут применяться в зависимости от вашей платформы, ознакомьтесь со статьей " [настраиваемые элементы везде](https://custom-elements-everywhere.com/) ".</span><span class="sxs-lookup"><span data-stu-id="31652-136">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="31652-137">В следующих разделах приводится краткий обзор использования компонентов набора инструментов Microsoft Graph с откликом и радиальным.</span><span class="sxs-lookup"><span data-stu-id="31652-137">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="31652-138">React</span><span class="sxs-lookup"><span data-stu-id="31652-138">React</span></span>

<span data-ttu-id="31652-139">Реагирует, что все данные передаются в настраиваемые элементы формы HTML Attributes.</span><span class="sxs-lookup"><span data-stu-id="31652-139">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="31652-140">Для примитивных данных это нормально, но не работает при передаче форматированных данных, таких как объекты или массивы.</span><span class="sxs-lookup"><span data-stu-id="31652-140">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="31652-141">В этих случаях для передачи объекта потребуется использовать `ref` объект.</span><span class="sxs-lookup"><span data-stu-id="31652-141">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="31652-142">Пример</span><span class="sxs-lookup"><span data-stu-id="31652-142">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="31652-143">Так как реакция реализует собственную виртуальную систему обработки событий, она не может прослушивать события модели DOM, поступающие из настраиваемых элементов, без использования обходного пути.</span><span class="sxs-lookup"><span data-stu-id="31652-143">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="31652-144">Необходимо использовать элемент a `ref` для ссылки на компоненты набора инструментов и вручную присоединить прослушиватели событий с помощью метода addEventListener, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="31652-144">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

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

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="31652-145">Реакция, typescript и целевой серверу</span><span class="sxs-lookup"><span data-stu-id="31652-145">React, Typescript, and TSX</span></span>

<span data-ttu-id="31652-146">Известная ошибка может возникать при использовании настраиваемых элементов с помощью реакции и typescript.</span><span class="sxs-lookup"><span data-stu-id="31652-146">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="31652-147">Typescript выдаст ошибку при попытке использовать компонент в целевом элементе.</span><span class="sxs-lookup"><span data-stu-id="31652-147">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="31652-148">Временное решение заключается в определении настраиваемого элемента в коде, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="31652-148">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="31652-149">Затем вы можете использовать его в целевом параметре как `<mgt-login></mgt-login>`.</span><span class="sxs-lookup"><span data-stu-id="31652-149">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="31652-150">Angular</span><span class="sxs-lookup"><span data-stu-id="31652-150">Angular</span></span>

<span data-ttu-id="31652-151">Синтаксис привязки по умолчанию в радиальной системе всегда будет задавайте свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="31652-151">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="31652-152">Это хорошо подходит для сложных данных, таких как объекты и массивы, а также для примитивных значений.</span><span class="sxs-lookup"><span data-stu-id="31652-152">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="31652-153">Прежде чем использовать настраиваемые элементы, включите в него `app.module.ts` `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator`настраиваемые элементы, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="31652-153">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

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

<span data-ttu-id="31652-154">Затем вы можете импортировать компонент, который вы хотите использовать, в файле Component \*. TS.</span><span class="sxs-lookup"><span data-stu-id="31652-154">You can then import the component you'd like to use in your component \*.ts file.</span></span>

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

<span data-ttu-id="31652-155">Наконец, используйте компонент, как обычно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="31652-155">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
