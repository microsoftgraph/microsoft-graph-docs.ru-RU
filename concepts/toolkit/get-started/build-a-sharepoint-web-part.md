---
title: Создание веб-части SharePoint с помощью Microsoft Graph Toolkit
description: Начало работы с Microsoft Graph Toolkit для создания веб-части SharePoint.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 700cfd44ddc115fc88451ce97880893b45feb9d3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588808"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Создание веб-части SharePoint с помощью Microsoft Graph Toolkit

В этом разделе рассказывается, как использовать компоненты Microsoft Graph Toolkit в [клиентской веб-части SharePoint](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts). Начало работы с включает следующие действия:

1. Настройка среды разработки и создание веб-части.
1. Добавление пакета SharePoint Framework Microsoft Graph Toolkit.
1. Добавление поставщика SharePoint.
1. Добавление компонентов.
1. Настройка разрешений.
1. Развертывание пакета SharePoint Framework Microsoft Graph Toolkit.
1. Создание и развертывание веб-части.
1. Проверка веб-части.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Настройка среды разработки SharePoint Framework и создание новой веб-части

Следуйте инструкциям о том, [Как настроить среду разработки SharePoint Framework](/sharepoint/dev/spfx/set-up-your-development-environment), а затем [создайте новую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Добавление пакета SharePoint Framework Microsoft Graph Toolkit

Чтобы несколько компонентов SharePoint Framework не регистрировали собственный набор компонентов Microsoft Graph Toolkit на странице, необходимо развернуть пакет SharePoint Framework Microsoft Graph Toolkit в клиенте и ссылаться на компоненты Microsoft Graph Toolkit, которые вы используете в решении из этого пакета.

Пакет SharePoint Framework Microsoft Graph Toolkit содержит библиотеку SharePoint Framework, которая регистрирует один экземпляр компонентов Microsoft Graph Toolkit в SharePoint.

Установите пакет NPM SharePoint Framework Microsoft Graph Toolkit с помощью следующей команды:

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>Добавление поставщика SharePoint

Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Веб-части SharePoint всегда существуют в контексте с проверкой подлинности, так как пользователю уже пришлось войти в систему, чтобы перейти на страницу, на которой размещена веб-часть. Используйте этот контекст для инициализации [поставщика SharePoint](../providers/sharepoint.md).

Сначала добавьте поставщика в веб-часть. Найдите файл `src\webparts\<your-project>\<your-web-part>.ts` в папке проекта и добавьте следующую строку в верхнюю часть файла прямо под существующими операторами `import` :

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

Затем необходимо инициализировать поставщика с контекстом проверки подлинности метода `onInit()` веб-части. В том же файле добавьте следующий код прямо перед строкой `public render(): void {`:

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>Добавление компонентов

Теперь можно приступить к добавлению компонентов в веб-часть. Просто добавьте компоненты в HTML-код внутри метода `render()`, и компоненты будут использовать контекст SharePoint для получения доступа к Microsoft Graph. Например, чтобы добавить [компонент "Человек"](../components/person.md), код будет выглядеть следующим образом:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> При создании веб-части с помощью React, ознакомьтесь с [документацией @microsoft/mgt-spfx](./mgt-spfx.md#react), чтобы узнать, как использовать `@microsoft/mgt-react`.

## <a name="configure-permissions"></a>Настройка разрешений

Чтобы вызвать Microsoft Graph из приложения SharePoint Framework, необходимо запросить необходимые разрешения в пакете решения, а администратор клиента Microsoft 365 должен утвердить запрошенные разрешения.

Чтобы добавить разрешения в пакет решения, найдите и откройте файл `config\package-solution.json`, а также настройте:

```json
"isDomainIsolated": false,
```

Под этой строкой добавьте следующее:

```json
"webApiPermissionRequests":[],
```

Определите необходимые разрешения API Microsoft Graph в зависимости от используемых компонентов. На странице документации каждого компонента содержится список разрешений, требуемых компоненту. Вам потребуется добавить каждое разрешение, необходимое для `webApiPermissionRequests`. Например, если вы используете компонент "Человек" и компонент "Повестка дня", `webApiPermissionRequests` может выглядеть следующим образом:

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Развертывание пакета SharePoint Framework Microsoft Graph Toolkit

Перед развертыванием пакета SharePoint Framework в клиенте необходимо развернуть пакет SharePoint Framework Microsoft Graph Toolkit на клиенте. Вы можете скачать пакет, соответствующий версии Microsoft Graph Toolkit, использованной в проекте, из раздела [Версии](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) на GitHub.

>[!IMPORTANT]
>Поскольку в клиенте может быть установлена только одна версия библиотеки SharePoint Framework для Microsoft Graph Toolkit, перед использованием Microsoft Graph Toolkit в решении определите, развернута ли в вашей организации или клиенте версия библиотеки SharePoint Framework и используется ли она.

После загрузки пакета SPPKG SharePoint Framework Microsoft Graph Toolkit, загрузите его в каталог приложений SharePoint Online. Перейдите на страницу [дополнительных функций Центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Выберите **Открыть** в разделе **Приложения**, а затем щелкните **Каталог приложений** и **Распространение приложений для SharePoint**. Загрузите файл `.sppkg` и нажмите кнопку **Развернуть**.

## <a name="build-and-deploy-your-web-part"></a>Создание и развертывание веб-части

Теперь вы создадите приложение и развернете его в SharePoint. Создайте приложение с помощью следующих команд:

```bash
gulp build
gulp bundle
gulp package-solution
```

В папке `sharepoint/solution` будет новый файл `.sppkg`. Вам потребуется отправить этот файл в каталог приложений SharePoint Online. Перейдите на страницу [дополнительных функций Центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Выберите **Открыть** в разделе **Приложения**, а затем щелкните **Каталог приложений** и **Распространение приложений для SharePoint**. Загрузите файл `.sppkg` и нажмите кнопку **Развернуть**.

Затем необходимо утвердить разрешения как администратор.

Перейдите в **Центр администрирования SharePoint**. В области навигации слева выберите **Дополнительно**, а затем **Доступ через API**. Вы должны увидеть ожидающие запросы для каждого из разрешений, которые были добавлены в файл `config\package-solution.json`. Выберите и утвердите каждое разрешение.

## <a name="test-your-web-part"></a>Проверка веб-части

Теперь вы готовы добавить веб-часть на страницу SharePoint и протестировать ее. Для тестирования веб-частей, использующих Microsoft Graph Toolkit, необходимо использовать размещенное рабочее место, так как для вызова Microsoft Graph компонентам требуется контекст проверки подлинности. Вы можете найти размещенное рабочее место на **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.

Откройте файл `config\serve.json` в проекте и замените значение `initialPage` URL-адресом размещенного рабочего места:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Сохраните файл и запустите следующую команду на консоли, чтобы создать и предварительно просмотреть веб-часть:

```bash
gulp serve
```

Размещенное рабочее место автоматически откроется в браузере. Добавьте веб-часть на страницу, и вы увидите ее вместе с компонентами Microsoft Graph Toolkit! Пока команда gulp serve все еще работает на консоли, можно продолжать вносить изменения в код, а затем просто обновлять браузер, чтобы увидеть изменения.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по SharePoint [веб-части](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
