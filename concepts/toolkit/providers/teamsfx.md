---
title: Поставщик TeamsFx
description: Используйте поставщик TeamsFx в приложениях Microsoft Teams, чтобы предоставить компонентам Microsoft Graph Toolkit доступ к Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 62df3d038c7a407da77e92b1d4de04fd1832aacf
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694396"
---
# <a name="teamsfx-provider"></a>Поставщик TeamsFx

Используйте поставщик TeamsFx в приложениях Microsoft Teams, чтобы предоставить компонентам Microsoft Graph Toolkit доступ к Microsoft Graph.

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы

Инициализировать поставщик внутри компонента.

```ts
// Import the providers and credential at the top of the page
import {Providers} from '@microsoft/mgt-element';
import {TeamsFxProvider} from '@microsoft/mgt-teamsfx-provider';
import {TeamsUserCredential} from "@microsoft/teamsfx";

const scope = ["User.Read"];
const teamsfx = new TeamsFx();
const provider = new TeamsFxProvider(teamsfx, scope);
Providers.globalProvider = provider;
```

Используйте этот `teamsfx.login(scopes)` метод для получения необходимого маркера доступа.

```ts
// Automatically when loading the component or in a call-to-action
await teamsfx.login(this.scope);
Providers.globalProvider.setState(ProviderState.SignedIn);
```

Теперь вы можете добавить любой компонент на HTML-странице `render()` или в метод при использовании React и использовать контекст TeamsFx для доступа к Microsoft Graph.

```html
<!-- Using HTML -->
<mgt-person query="me" view="threeLines"></mgt-person>
```

```ts
// Using React
public render(): void {
  return (
      <div>
        <Person personQuery="me" view={PersonViewType.threelines}></Person>
      </div>
  );
}
```

Пример, в котором показано, как инициализировать поставщика TeamsFx, см. в примере [экспорта контактов](https://github.com/OfficeDev/TeamsFx-Samples/tree/ga/graph-toolkit-contact-exporter).

## <a name="see-also"></a>См. также
* [начало работы разработки Microsoft Teams и Teams Toolkit](https://aka.ms/teamsfx-docs)
