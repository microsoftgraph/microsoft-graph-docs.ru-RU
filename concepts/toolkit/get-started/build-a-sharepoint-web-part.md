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
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Создайте SharePoint веб-часть с помощью microsoft Graph набор средств

В этом разделе описывается использование компонентов Microsoft Graph набор средств в SharePoint [клиентской веб-части](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts). Начало работы включает в себя следующие действия:

1. Настройка среды разработки и создание веб-части.
1. Добавьте пакет Microsoft Graph набор средств SharePoint Framework.
1. Добавьте SharePoint поставщика.
1. Добавление компонентов.
1. Настройка разрешений.
1. Развертывание пакета microsoft Graph набор средств SharePoint Framework.
1. Сборка и развертывание веб-части.
1. Проверьте веб-часть.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Настройка среды SharePoint Framework разработки и создание новой веб-части

Выполните действия по [настройкам среды SharePoint Framework разработки,](/sharepoint/dev/spfx/set-up-your-development-environment) а затем [создайте новую веб-часть.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Добавление пакета microsoft Graph набор средств SharePoint Framework

Чтобы не допустить SharePoint Framework компонентов Microsoft Graph набор средств на странице, необходимо развернуть пакет Microsoft Graph набор средств SharePoint Framework для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этого пакета.

Пакет Microsoft Graph набор средств SharePoint Framework содержит библиотеку SharePoint Framework, которая регистрирует один экземпляр компонентов Microsoft Graph набор средств в SharePoint.

Установите пакет microsoft Graph набор средств SharePoint Framework npm с помощью следующей команды:

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>Добавление SharePoint поставщика

Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). SharePoint веб-части всегда существуют в контексте проверки подлинности, так как пользователю уже пришлось войти, чтобы попасть на страницу, на которую размещена ваша веб-часть. Используйте этот контекст для инициализации [SharePoint поставщика](../providers/sharepoint.md).

Сначала добавьте поставщика в веб-часть. Найдите файл в папке проекта и добавьте следующую строку в верхнюю часть файла прямо под `src\webparts\<your-project>\<your-web-part>.ts` `import` существующими утверждениями:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

Далее необходимо инициализировать поставщика с помощью контекста проверки подлинности в `onInit()` методе веб-части. В том же файле добавьте следующий код прямо перед `public render(): void {` строкой:

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>Добавление компонентов

Теперь можно приступить к добавлению компонентов в веб-часть. Просто добавьте компоненты в HTML внутри метода, и компоненты будут использовать контекст SharePoint для доступа к `render()` Microsoft Graph. Например, чтобы добавить компонент [Person,](../components/person.md)код будет выглядеть так:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> Если вы строите веб-часть с React, см. в [@microsoft/mgt-spfx документы,](./mgt-spfx.md#react) чтобы узнать, как использовать `@microsoft/mgt-react` .

## <a name="configure-permissions"></a>Настройка разрешений

Чтобы вызвать microsoft Graph из SharePoint Framework приложения, необходимо запросить необходимые разрешения в пакете решений, а администратору Microsoft 365 необходимо утвердить запрашиваемую разрешения.

Чтобы добавить разрешения в пакет решений, найдите и откройте `config\package-solution.json` файл и установите:

```json
"isDomainIsolated": false,
```

Чуть ниже этой строки добавьте следующее:

```json
"webApiPermissionRequests":[],
```

Определите Graph разрешения API Майкрософт в зависимости от компонентов, которые вы используете. На странице документации каждого компонента содержится список разрешений, которые необходимы компоненту. Вам потребуется добавить каждое разрешение, необходимое `webApiPermissionRequests` для . Например, если вы используете компонент Person и компонент Agenda, вы можете `webApiPermissionRequests` выглядеть так:

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Развертывание пакета microsoft Graph набор средств SharePoint Framework

Перед развертывание SharePoint Framework пакета для клиента необходимо развернуть пакет Microsoft Graph набор средств SharePoint Framework для клиента. Вы можете скачать пакет, соответствующий версии microsoft Graph набор средств, используемой в [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) проекте, из раздела Выпуски на GitHub.

>[!IMPORTANT]
>Поскольку в клиенте SharePoint Framework может быть установлена только одна версия библиотеки Graph набор средств Microsoft, прежде чем использовать microsoft Graph набор средств в решении, определите, имеет ли ваша организация или клиент уже развернута версия библиотеки SharePoint Framework и использовать ту же версию.

Загрузив пакет Microsoft Graph набор средств SharePoint Framework sppkg, загрузите его в каталог SharePoint приложения. Перейдите на [страницу Дополнительные функции центра администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true) Выберите **Открыть** в **приложениях,** а затем нажмите **каталог приложений** и **раздать** приложения для SharePoint . Upload `.sppkg` файл и нажмите кнопку **Развертывание.**

## <a name="build-and-deploy-your-web-part"></a>Сборка и развертывание веб-части

Теперь вы создайте приложение и разверните его в SharePoint. Создайте приложение, запуская следующие команды:

```bash
gulp build
gulp bundle
gulp package-solution
```

В `sharepoint/solution` папке будет новый `.sppkg` файл. Вам потребуется загрузить этот файл в SharePoint каталога приложений в Интернете. Перейдите на [страницу Дополнительные функции центра администрирования SharePoint.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true) Выберите **Открыть** в **приложениях,** а затем нажмите **каталог приложений** и **раздать** приложения для SharePoint . Upload `.sppkg` файл и нажмите кнопку **Развертывание.**

Далее необходимо утвердить разрешения в качестве администратора.

Перейдите в **центр SharePoint администрирования.** В левой навигации выберите **Расширенный** и затем **API Access**. Вы должны видеть ожидающих запросов для каждого из разрешений, добавленных в `config\package-solution.json` файл. Выберите и утвердим каждое разрешение.

## <a name="test-your-web-part"></a>Проверка веб-части

Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Чтобы протестировать веб-части, которые используют microsoft Graph набор средств, необходимо использовать упорядоченный контекст, чтобы вызвать microsoft Graph. Вы можете найти у себя на сайте **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx.**

Откройте файл в проекте и замените значение URL-адресом для `config\serve.json` `initialPage` принимающей работы:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Сохраните файл и запустите следующую команду в консоли для создания и предварительного просмотра веб-части:

```bash
gulp serve
```

В браузере автоматически откроется хост-хозяйная работа. Добавьте веб-часть на страницу, и вы увидите веб-часть с компонентами Microsoft Graph набор средств в действии! До тех пор, пока команда службы глоток продолжает работать в консоли, вы можете продолжать вносить изменения в код, а затем просто обновить браузер, чтобы увидеть изменения.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по SharePoint [веб-части.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
