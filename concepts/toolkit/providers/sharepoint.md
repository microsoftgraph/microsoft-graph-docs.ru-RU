---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint для обеспечения доступа к компонентам с помощью Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: bb657e8fb5d6d9a775fb41e5c5c9fa6bf4662926
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657298"
---
# <a name="sharepoint-provider"></a>Поставщик SharePoint

Используйте поставщика SharePoint в веб-частях SharePoint для обеспечения доступа к компонентам с помощью Microsoft Graph.

Дополнительные информацию о поставщиках проверки подлинности см. [в этой теме.](./providers.md)

## <a name="get-started"></a>Начало работы

Инициализация поставщика в `onInit()` методе веб-части.

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

Теперь вы можете добавить в метод любой компонент, который будет использовать контекст `render()` SharePoint для доступа к Microsoft Graph.

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**Примечание.** Для набор средств Microsoft Graph требуется Typescript 3.x. Убедитесь, что вы используете поддерживаемую версию Typescript, [установив правильный компилятор.](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)

## <a name="sample"></a>Пример

Сведения о том, как инклиализировать поставщика SharePoint, см. в руководстве по началу работы с веб-частью "Создание веб-части [SharePoint".](../get-started/build-a-sharepoint-web-part.md)

Встроенный пример использования различных компонентов в веб-частях SharePoint см. в примере веб-части [SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории Microsoft Graph набор средств.

## <a name="test-in-the-workbench"></a>Тестирование в workbench

Если вы только начинаете работу с веб-частями SharePoint, вы можете следовать указаниям по созданию [первой веб-части.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)

После создания веб-части и готовности к использованию компонентов необходимо убедиться, что у веб-части есть необходимые разрешения на доступ к Microsoft Graph. Подробные сведения [см. в записи "Использовать Microsoft Graph" в SharePoint Framework.](/sharepoint/dev/spfx/use-aad-tutorial)

Одним словом, важно добавить в него нужное `package-solution.json` разрешение. Вам потребуется отправить пакет веб-части в SharePoint и попросить администратора утвердить запрашиваемую разрешения.

>[!TIP]
>Руководство по началу работы с веб-частью "Создание веб-части [SharePoint"](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговую инструкцию по настройке и одобрению разрешений.

>**Примечание.** Если вы не знаете, какие разрешения нужно добавить, документация для каждого компонента включает все необходимые ему разрешения.

## <a name="polyfills"></a>Polyfills

Если планируется поддержка IE11 в веб-части SPFx, необходимо использовать полизаполнеки.

Дополнительные данные [см. в этой](../get-started/overview.md#polyfills)набор средств.
