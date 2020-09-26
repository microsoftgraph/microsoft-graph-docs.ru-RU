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
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Создание веб-части SharePoint с помощью набора инструментов Microsoft Graph

В этом разделе описывается, как использовать компоненты набора инструментов Microsoft Graph в [клиентской веб-части SharePoint](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts). Приступая к работе состоит из следующих этапов:

1. Настройте среду разработки и создайте веб-часть.
2. Обновление TypeScript в проекте.
3. Добавьте набор инструментов Microsoft Graph.
4. Добавьте поставщика SharePoint.
5. Добавление компонентов.
6. Настройка разрешений.
7. Создание и развертывание веб-части.
8. Протестируйте веб-часть.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Настройка среды разработки SharePoint Framework и создание новой веб-части

Выполните действия, чтобы [настроить среду разработки SharePoint Framework](/sharepoint/dev/spfx/set-up-your-development-environment) , а затем [Создайте новую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

## <a name="update-typescript-in-your-project"></a>Обновление TypeScript в проекте

Набор средств Microsoft Graph требует typescript 3. x. Перед добавлением набора средств в проект убедитесь, что вы используете [поддерживаемую версию typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x). Например, чтобы добавить typescript 3,7, выполните следующую команду:

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
Затем найдите `tsconfig.json` файл в папке проекта, откройте файл и найдите следующую строку:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
Замените строку следующим:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление набора средств Microsoft Graph

Установите пакет инструментов набора инструментов Microsoft Graph NPM и с помощью следующей команды:

```bash
npm install @microsoft/mgt
```
Если вы планируете поддерживать IE11 в веб-частях, вам потребуется выполнить дополнительные действия, чтобы обеспечить совместимость между браузерами:

1. Установите следующие пакеты:
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. Добавьте следующий код в следующий код `gulpfile.js` `build.initialize(gulp)` :
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
3. В `src\webparts\<your-project>\<your-web-part>.ts` файле импортируйте указанные ниже операции с помощью оператора заполнил перед поставщиком SharePoint на следующем этапе.

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

## <a name="add-the-sharepoint-provider"></a>Добавление поставщика SharePoint

Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md). Веб-части SharePoint всегда существуют в контексте, прошедшем проверку подлинности, так как пользователь уже выполнил вход, чтобы перейти на страницу, на которой размещается веб-часть. Используйте этот контекст для инициализации [поставщика SharePoint](../providers/sharepoint.md).

Сначала добавьте поставщик в веб-часть. Выберите `src\webparts\<your-project>\<your-web-part>.ts` файл в папке проекта и добавьте следующую строку в верхнюю часть файла, расположенную ниже существующих `import` операторов:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

Далее необходимо инициализировать поставщика с помощью контекста, прошедшего проверку подлинности, в `onInit()` методе веб-части. В том же файле добавьте следующий код перед `public render(): void {` строкой:

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a>Добавление компонентов

Теперь можно приступить к добавлению компонентов в веб-часть. Просто добавьте компоненты в HTML-код в `render()` методе, и компоненты будут использовать контекст SharePoint для доступа к Microsoft Graph. Например, чтобы добавить [компонент Person](../components/person.md), ваш код будет выглядеть следующим образом:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a>Настройка разрешений

Для вызова Microsoft Graph из приложения SharePoint Framework необходимо запросить необходимые разрешения в пакете решения, а администратор клиента Microsoft 365 — утвердить запрошенные разрешения.

Чтобы добавить разрешения в пакет решения, перейдите к файлу и откройте его `config\package-solution.json` и задайте следующие настройки:

```json
"isDomainIsolated": false,
```

Под этой строкой добавьте следующий код:

```json
"webApiPermissionRequests":[],
```

Определите, какие разрешения API Microsoft Graph необходимы в зависимости от используемых компонентов. На странице документации каждого компонента представлен список разрешений, которые требуются компоненту. Вам потребуется добавить каждое разрешение, необходимое для `webApiPermissionRequests` . Например, если вы используете компонент Person и компонент повестки, он `webApiPermissionRequests` может выглядеть следующим образом:

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
## <a name="build-and-deploy-your-web-part"></a>Построение и развертывание веб-части

Теперь предстоит создать приложение и развернуть его в SharePoint. Постройте приложение, выполнив следующие команды:

```bash
gulp build
gulp bundle
gulp package-solution
```

В `sharepoint/solution` папке будет создан новый `.sppkg` файл. Вам потребуется загрузить этот файл в каталог приложений SharePoint Online. Перейдите на [страницу дополнительные компоненты своего центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Выберите пункт **Открыть** в разделе **приложения**, а затем выберите **Каталог приложений**и **Распространите приложения для SharePoint**. Отправьте `.sppkg` файл и нажмите кнопку **развернуть**.

Далее необходимо утвердить разрешения как администратор.

Перейдите в **центр администрирования SharePoint**. В левой области навигации выберите **Дополнительно** , а затем — **доступ к API**. Для каждого разрешения, добавленного в файл, должны отображаться ожидающие запросы `config\package-solution.json` . Выберите и утвердите каждое разрешение.

## <a name="test-your-web-part"></a>Тестирование веб-части

Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Для тестирования веб-частей, использующих набор инструментов Microsoft Graph, необходимо использовать размещенную рабочую среду, так как для вызова Microsoft Graph необходимо, чтобы для компонентов подлинность контекста была подлинной. Размещенный Workbench можно найти на сайте **https://<YOUR_TENANT>. SharePoint.com/_layouts/15/Workbench.aspx**.

Откройте `config\serve.json` файл в проекте и замените значение на `initialPage` URL-адрес размещенной рабочей области:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Сохраните файл, а затем выполните приведенную ниже команду в консоли, чтобы создать и просмотреть веб-часть:

```bash
gulp serve
```

Размещенная среда будет автоматически открываться в браузере. Добавьте веб-часть на страницу, и вы должны увидеть веб-часть с компонентами набора инструментов Microsoft Graph в действии! Пока команда gulp обслуживает все еще работает в консоли, вы можете продолжить внесение изменений в код, а затем просто обновить браузер, чтобы увидеть внесенные изменения.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми руководствами по [созданию веб-части SharePoint](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).
- Опробуйте компоненты в [интерактивная среда](https://mgt.dev).
- Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).
- Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).