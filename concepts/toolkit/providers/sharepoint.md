---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c27a24ac1b5f41b97d749620edbae09794072bed
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086755"
---
# <a name="sharepoint-provider"></a>Поставщик SharePoint

Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.

Чтобы узнать больше о поставщиках проверки подлинности, ознакомьтесь со статьей [поставщики](../providers.md).

## <a name="get-started"></a>Начало работы

Инициализируйте поставщик в `onInit()` методе веб-части.

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

Теперь вы можете добавить любой компонент в `render()` метод, который будет использовать контекст SharePoint для доступа к Microsoft Graph.

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**Примечание:** Набор средств Microsoft Graph требует typescript 3. x. Чтобы убедиться, что вы используете поддерживаемую версию typescript, [установите правильный компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).

## <a name="sample"></a>Пример

Подробнее о том, как инитализе поставщика SharePoint, можно узнать в статье Создание руководства по началу работы с [веб-частью SharePoint](../get-started/build-a-sharepoint-web-part.md) .

Предварительно созданный пример, в котором показано, как использовать различные компоненты в веб-частях SharePoint, можно найти в [примере веб-части SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории набора средств Microsoft Graph.

## <a name="test-in-the-workbench"></a>Тестирование в Workbench

Если вы только начинаете работать с веб-частями SharePoint, вы можете воспользоваться инструкциями по [созданию первой веб-части](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .

После создания веб-части и готовности к использованию компонентов необходимо убедиться, что веб-часть имеет необходимые разрешения для доступа к Microsoft Graph. Дополнительные сведения см. [в статье Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).

Коротко говоря, важно добавить правое разрешение для `package-solution.json` . Вам потребуется отправить пакет веб-части в SharePoint и разрешить администратору утверждать запрошенные разрешения.

>[!TIP]
>Руководство по началу работы с [веб-частью "Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) " содержит пошаговые инструкции по настройке и утверждению разрешений.

>**Примечание.** если вы не знаете, какие разрешения следует добавить, документация для каждого компонента включает все необходимые разрешения.

## <a name="polyfills"></a>Polyfills

Если вы планируете поддерживать IE11 в веб SPFx, необходимо использовать только.

Чтобы узнать больше, ознакомьтесь [со статьей начало работы с набором средств Microsoft Graph](../get-started/overview.md#polyfills).
