---
title: Библиотека SharePoint Framework для Microsoft Graph Toolkit
description: Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 952ff0852f4c1c0cf1efb2be2ab3cbe89d805f00
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588794"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>Библиотека SharePoint Framework для Microsoft Graph Toolkit

Используйте библиотеку SharePoint Framework microsoft Graph набор средств для использования Microsoft Graph набор средств в SharePoint Framework решениях.

Чтобы запретить нескольким компонентам регистрировать собственный набор компонентов Microsoft Graph набор средств на странице, следует развернуть эту библиотеку для клиента и ссылаться на компоненты Microsoft Graph набор средств, которые вы используете в решении из этой библиотеки.

> [!CAUTION]
> Библиотека SharePoint Framework microsoft Graph набор средств предназначена для использования с SharePoint Framework расширениями и не **изолированными веб-частями**. Если вы строите изолированные веб-части, не используйте библиотеку SharePoint Framework microsoft Graph набор средств. Вместо этого загрузим microsoft Graph набор средств непосредственно из пакета @microsoft/mgt (или @microsoft/mgt-react, если используется React). SharePoint Framework не поддерживает ссылки на компоненты библиотеки из изолированных веб-частей, что приведет к ошибкам во время работы в изолированной веб-части.

## <a name="installation"></a>Установка

Чтобы загрузить компоненты Microsoft Graph набор средств из библиотеки, `@microsoft/mgt-spfx` добавьте пакет в качестве зависимости от SharePoint Framework проекта:

```bash
npm install @microsoft/mgt-spfx
```

или

```bash
yarn add @microsoft/mgt-spfx
```

Перед развертывание SharePoint Framework пакета для клиента необходимо `@microsoft/mgt-spfx` развернуть SharePoint Framework для клиента. Пакет, соответствующий `@microsoft/mgt-spfx` версии, используемой в проекте, можно скачать в разделе Выпуски на [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) GitHub.

>[!IMPORTANT]
>Поскольку в клиенте может быть установлена только одна версия библиотеки SharePoint Framework для Microsoft Graph Toolkit, перед использованием Microsoft Graph Toolkit в решении определите, развернута ли в вашей организации или клиенте версия библиотеки SharePoint Framework и используется ли она.

## <a name="usage"></a>Применение

При создании SharePoint Framework веб-частей и расширений ссылайся на Graph набор средств Microsoft и `Provider` `SharePointProvider` из `@microsoft/mgt-spfx` пакета. Это позволит вашему решению использовать компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное их использование. Процесс мгновенной обработки является одинаковым для всех веб-частей независимо от используемой ими платформы JavaScript.

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

При создании веб-частей с помощью фреймворка, помимо React, можно загружать компоненты непосредственно в веб-части:

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

Если вы строите веб-часть с React, вы можете использовать `@microsoft/mgt-react` пакет. Однако не забудьте импортировать React компонентов с пути`@microsoft/mgt-react/dist/es6/spfx`. Это гарантирует, что ваше решение будет использовать только компоненты Microsoft Graph набор средств, которые уже зарегистрированы на странице, а не мгновенное ее собственное.

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
> Не импортируйте из других пакетов Microsoft Graph набор средств (`@microsoft/mgt-*`), чтобы избежать упаковки собственной копии инструментария и столкновения с общей библиотекой.

## <a name="see-also"></a>См. также

* [Создание веб-части SharePoint с помощью Microsoft Graph Toolkit](./build-a-sharepoint-web-part.md)
* [Сведения о поставщиках проверки подлинности](../providers/providers.md)
