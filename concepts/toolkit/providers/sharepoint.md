---
title: поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 684214e1490238564065c2ed53588b9700d17dc3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243076"
---
# <a name="sharepoint-provider"></a>поставщик SharePoint

Используйте поставщика SharePoint в веб-частях SharePoint, чтобы включить в себя доступ к компонентам Microsoft Graph.

Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).

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

## <a name="test-in-the-workbench"></a>Тестирование в Workbench

Если вы только начинаете работать с веб-частями SharePoint, вы можете воспользоваться инструкциями по [созданию первой веб-части](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .

После создания веб-части и готовности к использованию компонентов необходимо убедиться, что веб-часть имеет необходимые разрешения для доступа к Microsoft Graph. Дополнительные сведения см. [в статье Использование Microsoft Graph в SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial).

Коротко говоря, важно добавить правое разрешение для `package-solution.json`. Вам потребуется отправить пакет веб-части в SharePoint и разрешить администратору утверждать запрошенные разрешения.

>**Совет.** если вы не знаете, какие разрешения следует добавить, документация для каждого компонента включает все необходимые разрешения.
