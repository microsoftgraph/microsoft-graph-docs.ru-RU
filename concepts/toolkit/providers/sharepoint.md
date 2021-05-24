---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: eb5e5c5935e51fe7574c41feb57700f473567707
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629128"
---
# <a name="sharepoint-provider"></a>Поставщик SharePoint

Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы

Инициализируйте поставщика в методе `onInit()` веб-части. В этом примере используется [ `@microsoft/mgt-spfx` пакет](../get-started/mgt-spfx.md).

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

Теперь вы можете добавить любой компонент в метод `render()` и использовать контекст SharePoint для доступа к Microsoft Graph.

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

>**Примечание:** Microsoft Graph набор средств typescript 3.7 или более новый. Убедитесь, что вы используете поддерживаемую версию TypeScript, [установив соответствующий компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).

## <a name="sample"></a>Пример

Сведения о том, как инициализировать SharePoint поставщика, см. в руководстве [Сборка](../get-started/build-a-sharepoint-web-part.md) SharePoint веб-части.

## <a name="test-in-the-workbench"></a>Тестирование на рабочем месте

Если вы только начинаете работать с веб-частями SharePoint, следуйте руководству в статье [Создайте свою первую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

Когда вы создадите веб-часть и будете готовы использовать компоненты, убедитесь, что веб-часть имеет соответствующие разрешения для доступа к Microsoft Graph. Подробнее см. в статье [Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial)

Другими словами, к `package-solution.json` важно добавить соответствующее разрешение. Вам нужно будет отправить пакет веб-части в SharePoint, чтобы администратор утвердил запрошенные разрешения.

>[!TIP]
>Руководство по началу работы [Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговые инструкции по настройке и утверждению разрешений.

>**Примечание.** Если вы не знаете точно, какие разрешения следует добавить, все разрешения, необходимые для каждого компонента, указаны в документации по нему.