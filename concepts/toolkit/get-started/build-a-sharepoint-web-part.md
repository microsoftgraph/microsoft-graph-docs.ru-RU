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
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Создание веб-части SharePoint с помощью microsoft Graph набор средств

В этом разделе описывается, как использовать набор средств Microsoft Graph в клиентской [веб-части SharePoint.](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts) Начало работы состоит из следующих этапов:

1. Настройка среды разработки и создание веб-части.
2. Обновите TypeScript в проекте.
3. Добавьте microsoft Graph набор средств.
4. Добавьте поставщика SharePoint.
5. Добавление компонентов.
6. Настройка разрешений.
7. Создайте и разверните веб-часть.
8. Протестировать веб-часть.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Настройка среды разработки SharePoint Framework и создание новой веб-части

Выполните действия, [чтобы настроить среду разработки SharePoint Framework,](/sharepoint/dev/spfx/set-up-your-development-environment) а затем [создайте новую веб-часть.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)

## <a name="update-typescript-in-your-project"></a>Обновление TypeScript в проекте

Для набор средств Microsoft Graph требуется Typescript 3.x. Перед добавлением набор средств в проект убедитесь, что вы используете поддерживаемую [версию Typescript.](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x) Например, чтобы добавить Typescript 3.7, используйте следующую команду:

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
Затем найдите файл в папке проекта, откройте файл и найдите `tsconfig.json` эту строку:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
Замените строку на:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление учетной записи Microsoft Graph набор средств

Установите пакет и набор средств npm Microsoft Graph с помощью следующей команды:

```bash
npm install @microsoft/mgt
```
Если вы планируете поддерживать IE11 в веб-частях, вам потребуется предпринять дополнительные действия, чтобы обеспечить совместимость между браузерами:

1. Установите следующие пакеты:
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. Добавьте следующий код в `gulpfile.js` , прямо `build.initialize(gulp)` над:
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
3. В `src\webparts\<your-project>\<your-web-part>.ts` файле импортировать следующие полифайли перед поставщиком SharePoint на следующем шаге.

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

Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные узнать [см. в этой теме.](../providers/providers.md) Веб-части SharePoint всегда существуют в контексте с проверкой подлинности, так как пользователю уже пришлось войти на страницу, на которую размещена веб-часть. Используйте этот контекст для инициализации [поставщика SharePoint.](../providers/sharepoint.md)

Сначала добавьте поставщика в веб-часть. Найдите файл в папке проекта и добавьте следующую строку в верхнюю часть файла `src\webparts\<your-project>\<your-web-part>.ts` под существующими `import` строками:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

Затем необходимо инициализировать поставщика с контекстом проверки подлинности в `onInit()` методе веб-части. В том же файле добавьте следующий код прямо перед `public render(): void {` строкой:

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a>Добавление компонентов

Теперь можно приступить к добавлению компонентов в веб-часть. Просто добавьте компоненты в HTML-код внутри метода, и компоненты будут использовать контекст SharePoint для доступа `render()` к Microsoft Graph. Например, чтобы добавить компонент [Person,](../components/person.md)код будет выглядеть так:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a>Настройка разрешений

Чтобы вызвать Microsoft Graph из приложения SharePoint Framework, необходимо запросить необходимые разрешения в пакете решения, а администратор клиента Microsoft 365 должен утвердить запрашиваемую.

Чтобы добавить разрешения в пакет решения, найдите и откройте `config\package-solution.json` файл и установите:

```json
"isDomainIsolated": false,
```

Под этой строкой добавьте следующее:

```json
"webApiPermissionRequests":[],
```

Определите необходимые разрешения API Microsoft Graph в зависимости от используемого компонента. На странице документации каждого компонента содержится список разрешений, необходимых компоненту. Вам потребуется добавить каждое разрешение, необходимое для `webApiPermissionRequests` . Например, если вы используете компонент "Человек" и "Повестка дня", ваши задачи `webApiPermissionRequests` могут выглядеть так:

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
## <a name="build-and-deploy-your-web-part"></a>Создание и развертывание веб-части

Теперь вы создайте приложение и развернем его в SharePoint. Создайте приложение с помощью следующих команд:

```bash
gulp build
gulp bundle
gulp package-solution
```

В `sharepoint/solution` папке будет новый `.sppkg` файл. Вам потребуется отправить этот файл в каталог приложений SharePoint Online. Перейдите на [страницу "Дополнительные функции" в Центре администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true) Выберите **"Открыть** в **приложениях",** затем **"Каталог приложений"** и **"Распространение приложений для SharePoint".** Загрузите `.sppkg` файл и нажмите кнопку **"Развернуть".**

Затем необходимо утвердить разрешения от администратора.

Перейдите в **Центр администрирования SharePoint.** В области навигации слева выберите **"Расширенный",** а затем **"Доступ к API".** Должны отложенные запросы для каждого из разрешений, добавленных в `config\package-solution.json` файл. Выберите и утвердит каждое разрешение.

## <a name="test-your-web-part"></a>Тестирование веб-части

Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Для тестирования веб-частей, которые используют microsoft Graph набор средств, необходимо использовать веб-части с помощью веб-части с проверкой подлинности, так как для вызова Microsoft Graph компонентам необходим контекст проверки подлинности. Вы можете найти свою уехавную работу по адресу **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx.**

Откройте файл в проекте и замените значение URL-адреса для `config\serve.json` `initialPage` вашей хост-области:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Сохраните файл и запустите следующую команду в консоли, чтобы создать и просмотреть веб-часть:

```bash
gulp serve
```

В браузере будет автоматически открыта ваша уеханая работа. Добавьте веб-часть на страницу, и вы увидите ее с набор средств Microsoft Graph! Если команда gulp serve по-прежнему работает в консоли, вы можете продолжать вносить изменения в код, а затем просто обновлять браузер, чтобы увидеть изменения.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по [построению веб-части SharePoint.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)
- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)
- Сообщать об ошибках или оставлять запрос на функции на [GitHub.](https://aka.ms/mgt)