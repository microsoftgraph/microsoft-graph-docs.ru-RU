---
title: Person-Card компонента в microsoft Graph набор средств
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, связанных с человеком.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 79a14c3d37fba06a076e319b34029008b7fbf2fd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659185"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card компонента в microsoft Graph набор средств

Компонент Person-Card — это адаптивный компонент для отображения дополнительных сведений, связанных с человеком. Как правило, он используется в качестве flyout на `mgt-person` компоненте.

Дополнительные сведения о `mgt-person` компоненте см. [в mgt-person.](./person.md)

## <a name="example"></a>Пример

В следующем примере показано использование `mgt-person-card` компонента с `mgt-person` компонентом. Наведите курсор на человека, чтобы увидеть карточку [](#properties) человека, и используйте редактор кода, чтобы увидеть, как свойства изменяют поведение компонента.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a>Глобальная конфигурация компонентов

Класс `MgtPersonCard` предоставляет статический `config` объект, который настраивает все компоненты карточки человека в приложении. Объект config настраивает разделы и интерфейсы API, используемые карточкой пользователя для получения сведений о пользователе из Microsoft Graph.

По умолчанию все разделы и API включены. В следующем примере показано, как использовать объект config для отключения разделов или API.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

Для объекта config доступны следующие свойства.

| Свойство | Описание |
| ------------ | ------------- |
| useContactApis | `boolean` - Указывает, может ли компонент карточки человека использовать API контактов Microsoft Graph для поиска контактных данных и фотографий. Значение по умолчанию: `true`.  |
| sections | `object` - Настраивает разделы, которые будут показаны в карточке человека.  |

### <a name="person-card-sections"></a>Разделы карточки человека

Карточка человека содержит несколько настраиваемых разделов для отображения сведений о человеке:
* Contact - Contact information such as email, phone, position, location, and more.
* Организация — организационный график с руководителями, прямыми отчетами и соответствующими людьми.
* Сообщения — наиболее релевантные сообщения электронной почты с текущим во время вписаного пользователя.
* Файлы — наиболее релевантные общие файлы для текущего пользователя, выписав его.
* Профиль — сведения профиля, такие как проекты, навыки, языки и другие.

Разделы загружаются по умолчанию, но их можно отключить глобально с помощью `MgtPersonCard.config.sections` свойства объекта. Доступны следующие свойства.

| Свойство | Описание |
| ------------ | ------------- |
| organization; | `boolean` - Указывает, отображается ли раздел организации карточки человека. Значение по умолчанию: `true`.  |
| mailMessages | `boolean` - Указывает, отображается ли раздел сообщений карточки человека. Значение по умолчанию: `true`.  |
| files | `boolean` - Указывает, отображается ли раздел "Файлы карточки человека". Значение по умолчанию: `true`.  |
| profile | `boolean` - Указывает, отображается ли раздел профиля карточки пользователя. Значение по умолчанию: `true`.  |

Чтобы отключить раздел, просто задайте свойство в коде инициализации `false` приложения:.
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Настройка интеграции Teams

Компонент Person-Card позволяет пользователю связаться с целевым пользователем, в том числе с помощью чата Teams. Если компонент используется в приложении для вкладки Teams, можно убедиться, что компонент имеет прямую ссылку непосредственно на чат, а не открывает окно браузера, задав `microsoftTeamsLib` `TeamsProvider` его.

Если Person-Card не удается обнаружить lib Teams, он попытается открыть веб-клиент Teams.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

Дополнительные сведения о `TeamsProvider` поставщике см. в [сведениях о поставщике Microsoft Teams.](../providers/teams.md)

## <a name="properties"></a>Свойства

По умолчанию компонент передает сведения о `mgt-person` человеке `mgt-person-card` компоненту. Однако эти атрибуты можно использовать для изменения этого шаблона компонента или при использовании компонента в качестве `mgt-person` `mgt-person-card` автономного компонента.

| Атрибут         | Тип                     | Описание                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Объект Person, определенный в Microsoft Graph, содержащий сведения, связанные с пользователем. |
| person-image   | Строка                    | URI изображения, связанного с человеком, отображаемого на карточке.                                   |
| inherit-details   | Нет.                  | Позволяет карточке человека походить по родительскому дереву, чтобы компонент использует `mgt-person` те же данные и `person-details` `person-image` данные.                      |
| user-id | Строка | Позволяет разработчикам предоставить удостоверение пользователя для ирисовки данных, показанных в компоненте карточки пользователя |
| person-query | Строка | Позволяет разработчикам запрашивать данные, показанные в компоненте карточки пользователя |


## <a name="templates"></a>Шаблоны

Компонент Person-Card использует [шаблоны,](../customize-components/templates.md) позволяющие добавлять или заменять части компонента. Чтобы указать шаблон, включив элемент внутри компонента, закажите одно из `<template>` `data-type` следующих значений.

| Тип данных | Контекст данных | Описание |
| - | - | - |
| no-data | null | Шаблон, используемый, когда данные недоступны.
| default | `person`: объект сведений о человеке <br> `personImage`: URL-адрес изображения | Шаблон по умолчанию заменяет весь компонент на собственный. |
| person-details | `person`: объект сведений о человеке | Шаблон, используемый для отображения верхней части карточки человека. |
| additional-details | `person`: объект сведений о человеке <br> `personImage`: URL-адрес изображения | Шаблон, используемый для добавления пользовательского содержимого в контейнер дополнительных сведений. |

Например, можно использовать шаблон для настройки компонента, подключенного к компоненту, и шаблон для добавления дополнительных сведений `mgt-person` в карточку. 

```html
    <mgt-person person-query="me" view="twolines" person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-person-card` определяет следующие настраиваемые свойства CSS. 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
}
```

Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)

## <a name="microsoft-graph-apis-and-permissions"></a>API и разрешения Microsoft Graph

В Person-Card используются следующие API Microsoft Graph и разрешения.

| Ресурс | Разрешение | Раздел |
| - | - | - |
| [/me](/graph/api/user-get) | User.Read | По умолчанию |
| [/me/photo/$value](/graph/api/profilephoto-get) | User.Read | По умолчанию |
| [/me/people/?$search=](/graph/api/user-list-people) | People.Read | По умолчанию |
| [/me/contacts/\*](/graph/api/user-list-contacts) | Contacts.Read | По умолчанию |
| [/users/{id}](/graph/api/user-list-people) | User.ReadBasic.All | По умолчанию |
| [/users/{id}/photo/$value](/graph/api/profilephoto-get) | User.ReadBasic.All | По умолчанию |
| [/me/presence](/graph/api/presence-get) | Presence.Read | По умолчанию |
| [/users/{id}/presence](/graph/api/presence-get) | Presence.Read.All | По умолчанию |
| [/users/{id}/manager](/graph/api/user-list-manager) | User.Read.All | Организация |
| [/users/{id}/directReports](/graph/api/user-list-directreports) | User.Read.All | Организация |
| [/users/{id}/people](/graph/api/user-list-people) | People.Read.All | Организация |
| [/me/messages](/graph/api/user-list-messages) | Mail.ReadBasic | Сообщения |
| [/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used) | Sites.Read.All | Файлы |
| [/users/{id}/profile](/graph/api/profile-get) | User.Read.All | Профиль |

Класс также предоставляет статический метод, который возвращает массив областей, необходимых для работы карточки человека на основе глобальной конфигурации `MgtPersonCard` `getScopes` карточки человека.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Проверка подлинности

В Person-Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md) 
