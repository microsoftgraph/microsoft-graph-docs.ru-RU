---
title: SharePoint Framework для Microsoft Graph набор средств
description: Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 17a6e899003dec34a6dac41daaeba7e2c0e3fba1
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579876"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>SharePoint Framework для Microsoft Graph набор средств

Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.

Чтобы запретить нескольким компонентам регистрировать собственный набор компонентов Microsoft Graph набор средств на странице, следует развернуть эту библиотеку для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этой библиотеки.

## <a name="installation"></a>Установка

Чтобы загрузить компоненты microsoft Graph набор средств из библиотеки, добавьте пакет в качестве зависимости от времени работы в `@microsoft/mgt-spfx` SharePoint Framework проект:

```bash
npm install @microsoft/mgt-spfx
```

или

```bash
yarn add @microsoft/mgt-spfx
```

Перед развертывание SharePoint Framework пакета для клиента необходимо развернуть SharePoint Framework `@microsoft/mgt-spfx` для клиента. Вы можете скачать пакет, соответствующий версии, используемой в проекте, из раздела `@microsoft/mgt-spfx` [Выпуски](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) на GitHub.

>[!IMPORTANT]
>Поскольку в клиенте SharePoint Framework может быть установлена только одна версия библиотеки Graph набор средств Microsoft, прежде чем использовать microsoft Graph набор средств в решении, определите, имеет ли ваша организация или клиент уже развернута версия библиотеки SharePoint Framework и использовать ту же версию.

## <a name="usage"></a>Usage

При создании SharePoint Framework веб-частей и расширений ссылайся на microsoft Graph набор средств `Provider` и `SharePointProvider` из `@microsoft/mgt-spfx` пакета. Это позволит вашему решению использовать компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное их использование. Процесс мгновенной обработки является одинаковым для всех веб-частей независимо от используемой ими платформы JavaScript.

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtWebPart extends BaseClientSideWebPart<IMgtWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  // [...] trimmed for brevity
}
```

При создании веб-частей с помощью фреймворка, кроме React, можно загружать компоненты непосредственно в веб-части:

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div class="${styles.mgtNoFramework}">
        <div class="${styles.container}">
          <div class="${styles.row}">
            <div class="${styles.column}">
              <span class="${styles.title}">No framework webpart</span>
              <mgt-person person-query="me" show-name show-email></mgt-person>
            </div>
          </div>
        </div>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

Если вы создаете веб-часть с React, загружайте компоненты из `@microsoft/mgt-react` пакета:

```tsx
import { Person } from '@microsoft/mgt-react';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" />
      </div>
    );
  }
}
```

## <a name="see-also"></a>См. также

* [Создайте SharePoint веб-часть с помощью microsoft Graph набор средств](./build-a-sharepoint-web-part.md)
* [Сведения о поставщиках проверки подлинности](../providers/providers.md)
