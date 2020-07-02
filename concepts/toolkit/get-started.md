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
# <a name="get-started-with-the-microsoft-graph-toolkit"></a>Начало работы с набором средств Microsoft Graph

Набор средств Microsoft Graph можно легко включить в веб-приложение, веб-часть SharePoint или на вкладку Microsoft Teams. Компоненты основаны на существующих веб-стандартах и совместимы с любой веб-средой и современным браузером. В этом разделе описывается, как приступить к использованию набора средств Microsoft Graph в проекте.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.

## <a name="use-via-mgt-loader"></a>Использование с помощью упр. загрузчиком

Для использования набора средств с помощью средства управления "центр управления" обратитесь к следующему примеру.

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

Затем можно использовать компоненты на HTML-странице. Ниже приведен полный рабочий пример с поставщиком MSAL.

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> **Примечание:** Для перенаправления проверки подлинности MSAL необходимо, чтобы страница была размещена на веб-сервере. Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code.

## <a name="use-via-npm-es6-modules"></a>Использование через NPM (модули ES6)

С помощью модулей ES6 вы можете получить полный доступ к процессу объединения, и вы можете объединить только код, который требуется для вашего сайта. Сначала добавьте пакет NPM:

```bash
npm install @microsoft/mgt
```

Теперь вы можете ссылаться на все компоненты на странице, которую вы используете:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

Аналогичным образом, чтобы добавить поставщика, можно добавить его в качестве компонента:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

Или добавьте его в код:

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a>Поставщики

Компоненты лучше всего подходят для использования с [поставщиками](./providers.md). Поставщик предоставляет доступ к проверке подлинности и интерфейсам API, которые используются компонентами для вызова Microsoft Graph.

Набор средств содержит поставщики для [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md)и [Teams](./providers/teams.md). Вы также можете использовать собственную логику проверки подлинности, создав [настраиваемый поставщик](./providers/custom.md)или используя [проксипровидер](./providers/proxy.md) с собственной внутренней проверкой подлинности. 

## <a name="polyfills"></a>Polyfills

Если вы используете модули ES6 из пакета NPM, не забудьте включить в проект только те, которые не включены автоматически. Дополнительные сведения [см.](https://www.webcomponents.org/polyfills)

Если вы используете mgt-loader.js скрипт из пакета в унпкг, то эти функции уже включены.

### <a name="sharepoint"></a>SharePoint

Если вы планируете поддерживать IE11 в веб SPFx, в следующей процедуре описаны действия, необходимые для обеспечения совместимости между браузерами: 

1. Установите следующие пакеты:
```cmd
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
npm install @microsoft/mgt
```

2. Вставьте следующий файл конфигурации в gulpfile.js над build.iniтиалзе (gulp);
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


3. В файле * WebPart. TS импортируйте указанные ниже части перед импортом поставщиков.
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

Дополнительные сведения см. в разделе [поставщик SharePoint](./providers/sharepoint.md).

## <a name="using-the-components-with-react-angular-and-other-frameworks"></a>Использование компонентов с реагирует, радиально и другими платформами

Веб-компоненты основываются на нескольких веб-стандартах и могут использоваться с любой уже используемой платформой. Однако не все платформы обрабатывают веб-компоненты одинаковым образом. Чтобы узнать больше о возможностях, которые могут применяться в зависимости от вашей платформы, ознакомьтесь со статьей " [настраиваемые элементы везде](https://custom-elements-everywhere.com/) ".

В следующих разделах приводится краткий обзор использования компонентов набора инструментов Microsoft Graph с откликом и радиальным.

### <a name="react"></a>React

Реагирует, что все данные передаются в настраиваемые элементы формы HTML Attributes. Для примитивных данных это нормально, но не работает при передаче форматированных данных, таких как объекты или массивы. В этих случаях для передачи объекта потребуется использовать объект `ref` .

Пример

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

Так как реакция реализует собственную виртуальную систему обработки событий, она не может прослушивать события модели DOM, поступающие из настраиваемых элементов, без использования обходного пути. Необходимо использовать элемент a `ref` для ссылки на компоненты набора инструментов и вручную присоединить прослушиватели событий с помощью метода addEventListener, как показано в следующем примере.

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

#### <a name="react-typescript-and-tsx"></a>Реакция, typescript и целевой серверу

Известная ошибка может возникать при использовании настраиваемых элементов с помощью реакции и typescript. Typescript выдаст ошибку при попытке использовать компонент в целевом элементе. Временное решение заключается в определении настраиваемого элемента в коде, как показано ниже.

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

Затем вы можете использовать его в целевом параметре как `<mgt-login></mgt-login>` .

### <a name="angular"></a>Angular

Синтаксис привязки по умолчанию в радиальной системе всегда будет задавайте свойства элемента. Это хорошо подходит для сложных данных, таких как объекты и массивы, а также для примитивных значений.

Прежде чем использовать настраиваемые элементы, включите в него настраиваемые элементы `app.module.ts` `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` , как показано в следующем примере.

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

Затем вы можете импортировать компонент, который вы хотите использовать, в файле Component \* . TS.

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

Наконец, используйте компонент, как обычно в шаблоне.

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```

