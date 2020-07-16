---
title: Начало работы с набором средств Microsoft Graph
description: Приступите к работе с набором инструментов Microsoft Toolkit в вашем приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2e352a71b7e1f068bfb6dbd13a6ed151dd1b84b0
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007068"
---
# <a name="get-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="1ba70-103">Начало работы с набором средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1ba70-103">Get started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1ba70-104">Набор средств Microsoft Graph можно легко включить в веб-приложение, веб-часть SharePoint или на вкладку Microsoft Teams. Компоненты основаны на существующих веб-стандартах и совместимы с любой веб-средой и современным браузером.</span><span class="sxs-lookup"><span data-stu-id="1ba70-104">The Microsoft Graph Toolkit can easily be included in your web application, SharePoint web part, or Microsoft Teams tab. The components are built on existing web standards and are compatible with any web framework and modern browser.</span></span> <span data-ttu-id="1ba70-105">В этом разделе описывается, как приступить к использованию набора средств Microsoft Graph в проекте.</span><span class="sxs-lookup"><span data-stu-id="1ba70-105">This topic describes how to get started using the Microsoft Graph Toolkit in your project.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="1ba70-106">Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.</span><span class="sxs-lookup"><span data-stu-id="1ba70-106">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

## <a name="use-via-mgt-loader"></a><span data-ttu-id="1ba70-107">Использование с помощью упр. загрузчиком</span><span class="sxs-lookup"><span data-stu-id="1ba70-107">Use via mgt-loader</span></span>

<span data-ttu-id="1ba70-108">Для использования набора средств с помощью средства управления "центр управления" обратитесь к следующему примеру.</span><span class="sxs-lookup"><span data-stu-id="1ba70-108">To use the toolkit via mgt-loader, see the following example.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="1ba70-109">Затем можно использовать компоненты на HTML-странице.</span><span class="sxs-lookup"><span data-stu-id="1ba70-109">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="1ba70-110">Ниже приведен полный рабочий пример с поставщиком MSAL.</span><span class="sxs-lookup"><span data-stu-id="1ba70-110">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="1ba70-111">**Примечание:** Для перенаправления проверки подлинности MSAL необходимо, чтобы страница была размещена на веб-сервере.</span><span class="sxs-lookup"><span data-stu-id="1ba70-111">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="1ba70-112">Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="1ba70-112">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

## <a name="use-via-npm-es6-modules"></a><span data-ttu-id="1ba70-113">Использование через NPM (модули ES6)</span><span class="sxs-lookup"><span data-stu-id="1ba70-113">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="1ba70-114">С помощью модулей ES6 вы можете получить полный доступ к процессу объединения, и вы можете объединить только код, который требуется для вашего сайта.</span><span class="sxs-lookup"><span data-stu-id="1ba70-114">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="1ba70-115">Сначала добавьте пакет NPM:</span><span class="sxs-lookup"><span data-stu-id="1ba70-115">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="1ba70-116">Теперь вы можете ссылаться на все компоненты на странице, которую вы используете:</span><span class="sxs-lookup"><span data-stu-id="1ba70-116">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="1ba70-117">Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:</span><span class="sxs-lookup"><span data-stu-id="1ba70-117">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="1ba70-118">Аналогичным образом, чтобы добавить поставщика, можно добавить его в качестве компонента:</span><span class="sxs-lookup"><span data-stu-id="1ba70-118">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="1ba70-119">Или добавьте его в код:</span><span class="sxs-lookup"><span data-stu-id="1ba70-119">Or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="1ba70-120">Поставщики</span><span class="sxs-lookup"><span data-stu-id="1ba70-120">Providers</span></span>

<span data-ttu-id="1ba70-121">Компоненты лучше всего подходят для использования с [поставщиками](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="1ba70-121">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="1ba70-122">Поставщик предоставляет доступ к проверке подлинности и интерфейсам API, которые используются компонентами для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1ba70-122">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="1ba70-123">Набор средств содержит поставщики для [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md)и [Teams](./providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="1ba70-123">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), and [Teams](./providers/teams.md).</span></span> <span data-ttu-id="1ba70-124">Вы также можете использовать собственную логику проверки подлинности, создав [настраиваемый поставщик](./providers/custom.md)или используя [проксипровидер](./providers/proxy.md) с собственной внутренней проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="1ba70-124">You can also use your own authentication logic by creating a [custom provider](./providers/custom.md), or using the [ProxyProvider](./providers/proxy.md) with your own backend authentication.</span></span> 

## <a name="polyfills"></a><span data-ttu-id="1ba70-125">Polyfills</span><span class="sxs-lookup"><span data-stu-id="1ba70-125">Polyfills</span></span>

<span data-ttu-id="1ba70-126">Если вы используете модули ES6 из пакета NPM, не забудьте включить в проект только те, которые не включены автоматически.</span><span class="sxs-lookup"><span data-stu-id="1ba70-126">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="1ba70-127">Дополнительные сведения [см.](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="1ba70-127">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="1ba70-128">Если вы используете mgt-loader.js скрипт из пакета в унпкг, то эти функции уже включены.</span><span class="sxs-lookup"><span data-stu-id="1ba70-128">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>

### <a name="sharepoint"></a><span data-ttu-id="1ba70-129">SharePoint</span><span class="sxs-lookup"><span data-stu-id="1ba70-129">Sharepoint</span></span>

<span data-ttu-id="1ba70-130">Если вы планируете поддерживать IE11 в веб SPFx, в следующей процедуре описаны действия, необходимые для обеспечения совместимости между браузерами:</span><span class="sxs-lookup"><span data-stu-id="1ba70-130">If you plan to support IE11 in your SPFx webparts, the following process describes the necessary steps to ensure cross-browser compatibility:</span></span> 

1. <span data-ttu-id="1ba70-131">Установите следующие пакеты:</span><span class="sxs-lookup"><span data-stu-id="1ba70-131">Install the following packages:</span></span>
```cmd
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
npm install @microsoft/mgt
```

2. <span data-ttu-id="1ba70-132">Вставьте следующий файл конфигурации в gulpfile.js над build.iniтиалзе (gulp);</span><span class="sxs-lookup"><span data-stu-id="1ba70-132">Insert the following config in your gulpfile.js just above your build.initialze(gulp);</span></span>
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


3. <span data-ttu-id="1ba70-133">В файле \* WebPart. TS импортируйте указанные ниже части перед импортом поставщиков.</span><span class="sxs-lookup"><span data-stu-id="1ba70-133">In your \*WebPart.ts file, import the following polyfills before import of the providers</span></span>
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

<span data-ttu-id="1ba70-134">Дополнительные сведения см. в разделе [поставщик SharePoint](./providers/sharepoint.md).</span><span class="sxs-lookup"><span data-stu-id="1ba70-134">To learn more, see [sharepoint provider](./providers/sharepoint.md).</span></span>

## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="1ba70-135">Использование компонентов с реагирует, радиально и другими платформами</span><span class="sxs-lookup"><span data-stu-id="1ba70-135">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="1ba70-136">Веб-компоненты основываются на нескольких веб-стандартах и могут использоваться с любой уже используемой платформой.</span><span class="sxs-lookup"><span data-stu-id="1ba70-136">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="1ba70-137">Однако не все платформы обрабатывают веб-компоненты одинаковым образом.</span><span class="sxs-lookup"><span data-stu-id="1ba70-137">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="1ba70-138">Чтобы узнать больше о возможностях, которые могут применяться в зависимости от вашей платформы, ознакомьтесь со статьей " [настраиваемые элементы везде](https://custom-elements-everywhere.com/) ".</span><span class="sxs-lookup"><span data-stu-id="1ba70-138">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="1ba70-139">В следующих разделах приводится краткий обзор использования компонентов набора инструментов Microsoft Graph с откликом и радиальным.</span><span class="sxs-lookup"><span data-stu-id="1ba70-139">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="1ba70-140">React</span><span class="sxs-lookup"><span data-stu-id="1ba70-140">React</span></span>

<span data-ttu-id="1ba70-141">Реагирует, что все данные передаются в настраиваемые элементы формы HTML Attributes.</span><span class="sxs-lookup"><span data-stu-id="1ba70-141">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="1ba70-142">Для примитивных данных это нормально, но не работает при передаче форматированных данных, таких как объекты или массивы.</span><span class="sxs-lookup"><span data-stu-id="1ba70-142">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="1ba70-143">В этих случаях для передачи объекта потребуется использовать объект `ref` .</span><span class="sxs-lookup"><span data-stu-id="1ba70-143">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="1ba70-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1ba70-144">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="1ba70-145">Так как реакция реализует собственную виртуальную систему обработки событий, она не может прослушивать события модели DOM, поступающие из настраиваемых элементов, без использования обходного пути.</span><span class="sxs-lookup"><span data-stu-id="1ba70-145">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="1ba70-146">Необходимо использовать элемент a `ref` для ссылки на компоненты набора инструментов и вручную присоединить прослушиватели событий с помощью метода addEventListener, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="1ba70-146">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

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

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="1ba70-147">Реакция, typescript и целевой серверу</span><span class="sxs-lookup"><span data-stu-id="1ba70-147">React, Typescript, and TSX</span></span>

<span data-ttu-id="1ba70-148">Известная ошибка может возникать при использовании настраиваемых элементов с помощью реакции и typescript.</span><span class="sxs-lookup"><span data-stu-id="1ba70-148">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="1ba70-149">Typescript выдаст ошибку при попытке использовать компонент в целевом элементе.</span><span class="sxs-lookup"><span data-stu-id="1ba70-149">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="1ba70-150">Временное решение заключается в определении настраиваемого элемента в коде, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="1ba70-150">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="1ba70-151">Затем вы можете использовать его в целевом параметре как `<mgt-login></mgt-login>` .</span><span class="sxs-lookup"><span data-stu-id="1ba70-151">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="1ba70-152">Angular</span><span class="sxs-lookup"><span data-stu-id="1ba70-152">Angular</span></span>

<span data-ttu-id="1ba70-153">Синтаксис привязки по умолчанию в радиальной системе всегда будет задавайте свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="1ba70-153">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="1ba70-154">Это хорошо подходит для сложных данных, таких как объекты и массивы, а также для примитивных значений.</span><span class="sxs-lookup"><span data-stu-id="1ba70-154">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="1ba70-155">Прежде чем использовать настраиваемые элементы, включите в него настраиваемые элементы `app.module.ts` `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="1ba70-155">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

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

<span data-ttu-id="1ba70-156">Затем вы можете импортировать компонент, который вы хотите использовать, в файле Component \* . TS.</span><span class="sxs-lookup"><span data-stu-id="1ba70-156">You can then import the component you'd like to use in your component \*.ts file.</span></span>

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

<span data-ttu-id="1ba70-157">Наконец, используйте компонент, как обычно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="1ba70-157">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```

