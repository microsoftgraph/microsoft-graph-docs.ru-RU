---
title: Поставщик SharePoint
description: Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 2dc020dbe02a5b3018c1bfb343b7582f8a6110e5
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072347"
---
# <a name="sharepoint-provider"></a>Поставщик SharePoint

Используйте поставщика SharePoint в веб-частях SharePoint, чтобы предоставить компонентам доступ к Microsoft Graph.

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы

Инициализируйте поставщика в методе `onInit()` веб-части.

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

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

>**Примечание.** Microsoft Graph Toolkit требует использования TypeScript 3.x. Убедитесь, что вы используете поддерживаемую версию TypeScript, [установив соответствующий компилятор](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).

## <a name="sample"></a>Пример

Сведения о том, как инициализировать поставщика SharePoint, см. в руководстве по началу работы с веб-частью "Создание веб-части [SharePoint".](../get-started/build-a-sharepoint-web-part.md)

Пример готовой веб-части, в котором показано, как использовать различные компоненты в веб-частях SharePoint, см. в статье [Пример веб-части SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) в репозитории Microsoft Graph Toolkit.

## <a name="test-in-the-workbench"></a>Тестирование на рабочем месте

Если вы только начинаете работать с веб-частями SharePoint, следуйте руководству в статье [Создайте свою первую веб-часть](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

Когда вы создадите веб-часть и будете готовы использовать компоненты, убедитесь, что веб-часть имеет соответствующие разрешения для доступа к Microsoft Graph. Подробнее см. в статье [Использование Microsoft Graph в SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial)

Другими словами, к `package-solution.json` важно добавить соответствующее разрешение. Вам нужно будет отправить пакет веб-части в SharePoint, чтобы администратор утвердил запрошенные разрешения.

>[!TIP]
>Руководство по началу работы [Создание веб-части SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) содержит пошаговые инструкции по настройке и утверждению разрешений.

>**Примечание.** Если вы не знаете точно, какие разрешения следует добавить, все разрешения, необходимые для каждого компонента, указаны в документации по нему.

## <a name="polyfills"></a>Полизаполнение

Если вы планируете поддерживать IE11 в веб-частях SPFx, необходимо использовать полизаполнение.

Дополнительные сведения см. в статье [Начало работы с Microsoft Graph Toolkit](../get-started/overview.md#polyfills).
