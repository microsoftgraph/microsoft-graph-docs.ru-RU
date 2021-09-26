---
title: Библиотека SharePoint Framework для Microsoft Graph Toolkit
description: Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.
ms.localizationpriority: medium
author: waldekmastykarz
ms.openlocfilehash: 41a1b3703440ce42866c3aaf720bdda55e9d2b20
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507762"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>Библиотека SharePoint Framework для Microsoft Graph Toolkit

Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.

Чтобы запретить нескольким компонентам регистрировать собственный набор компонентов Microsoft Graph набор средств на странице, следует развернуть эту библиотеку для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этой библиотеки.

> [!CAUTION]
> Библиотека SharePoint Framework microsoft Graph набор средств предназначена для использования с SharePoint Framework расширениями и не **изолированными веб-частями.** Если вы строите изолированные веб-части, не используйте библиотеку SharePoint Framework для microsoft Graph набор средств. Вместо этого загрузим microsoft Graph набор средств непосредственно из пакета @microsoft/mgt (или @microsoft/mgt-react при использовании React). SharePoint Framework не поддерживает компоненты библиотеки ссылок из изолированных веб-частей, и это приведет к ошибкам во время работы в изолированной веб-части.

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
>Поскольку в клиенте может быть установлена только одна версия библиотеки SharePoint Framework для Microsoft Graph Toolkit, перед использованием Microsoft Graph Toolkit в решении определите, развернута ли в вашей организации или клиенте версия библиотеки SharePoint Framework и используется ли она.

## <a name="usage"></a>Использование

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
      <div>
        <mgt-person person-query="me"></mgt-person>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

### <a name="react"></a>React

Если вы строите веб-часть с React, вы можете использовать `@microsoft/mgt-react` пакет. Однако не забудьте импортировать React компонентов с `@microsoft/mgt-react/dist/es6/spfx` пути. Это гарантирует, что ваше решение будет использовать только компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное ее собственное.

```tsx
import { Person } from '@microsoft/mgt-react/dist/es6/spfx';
import { ViewType } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" view={ViewType.image}></Person>
      </div>
    );
  }
}
```

>[!IMPORTANT]
> Убедитесь, что все Graph набор средств Майкрософт в вашем решении являются либо из:
> * `@microsoft/mgt-spfx` или
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> Не импортируйте из других пакетов Microsoft Graph набор средств (), чтобы избежать упаковки собственной копии инструментария и столкновения с `@microsoft/mgt-*` общей библиотекой.

## <a name="see-also"></a>См. также

* [Создание веб-части SharePoint с помощью Microsoft Graph Toolkit](./build-a-sharepoint-web-part.md)
* [Сведения о поставщиках проверки подлинности](../providers/providers.md)
