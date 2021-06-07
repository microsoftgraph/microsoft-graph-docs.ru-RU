---
title: Компонент Person-Card в Microsoft Graph Toolkit
description: Компонент Person-Card для просмотра дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 8497dbb3b3d9a3173cdbf8ee8ec6bfe74859868b
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780703"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Компонент Person-Card в Microsoft Graph Toolkit

Компонент Person-Card — это адаптивный компонент для просмотра дополнительных сведений, относящихся к пользователю. Обычно используется в качестве всплывающего окна для компонента `mgt-person`.

Дополнительные сведения о компоненте `mgt-person` см. в разделе [mgt-person](./person.md).

## <a name="example"></a>Пример

В приведенном ниже примере показано использование компонента `mgt-person-card` с компонентом `mgt-person`. Наведите указатель мыши на человека, чтобы увидеть карточку контакта, а затем в редакторе кода посмотрите, как [свойства](#properties) изменить поведение компонента.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a>Настройка глобального компонента

Класс `MgtPersonCard` предоставляет статический объект `config`, который конфигурирует все компоненты карточки контакта в приложении. В объекте config настраивается, какие разделы и какие API-интерфейсы используются для получения сведений о пользователе в Microsoft Graph.

По умолчанию все разделы и API-интерфейсы включены. В приведенном ниже примере показано, как использовать объект конфигурации для отключения разделов и API-интерфейсов.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

Ниже указаны свойства, доступные в объекте конфигурации.

| Свойство | Описание |
| ------------ | ------------- |
| useContactApis | `boolean` — Указывает, может ли компонент карточки контакта использовать API контактов Microsoft Graph для поиска контактных данных и фотографий. Значение по умолчанию: `true`.  |
| sections | `object` — Настройка отображения разделов в карточке контакта.  |

### <a name="person-card-sections"></a>Разделы карточки контакта

Карточка контакта содержит несколько настраиваемых разделов, в которых отображаются сведения о пользователе:
* Контакт — контактные данные, такие как электронная почта, номер телефона, должность, расположение и другие сведения.
* Организация — организационная диаграмма с руководителями, подчиненными или важными пользователями.
* Сообщения — наиболее актуальные сообщения электронной почты вошедшего в систему пользователя.
* Файлы — наиболее актуальные общие файлы вошедшего в систему пользователя.
* Профиль — информация о профиле, например проекты, навыки, языки и другие сведения.

Разделы загружаются по умолчанию, но их можно отключить глобально с помощью свойства объекта `MgtPersonCard.config.sections`. Для редактирования доступны следующие свойства.

| Свойство | Описание |
| ------------ | ------------- |
| organization; | `boolean` — указывает, отображается ли раздел организации карточки контакта. Значение по умолчанию: `true`.  |
| mailMessages | `boolean` — указывает, отображается ли раздел сообщений карточки контакта. Значение по умолчанию: `true`.  |
| files | `boolean` — указывает, отображается ли раздела файлов карточки контакта. Значение по умолчанию: `true`.  |
| profile | `boolean` — указывает, отображается ли раздел профиля карточки контакта. Значение по умолчанию: `true`.  |

Чтобы отключить раздел, просто установите свойство в коде инициализации `false` приложения:
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Настройка интеграции с Teams

Компонент Person-Card позволяет связаться с целевым контактом, в том числе с помощью чата в Teams. При использовании компонента во вкладке приложения Teams можно сделать так, чтобы компонент не открывал окно браузера, а сразу переходил к чату, настроив `microsoftTeamsLib` в `TeamsProvider`.

Если компоненту Person-Card не удается обнаружить библиотеку Teams, компонент пытается открыть веб-клиент Teams.

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

Дополнительные сведения о поставщике `TeamsProvider` см. в статье ["Поставщик Microsoft Teams"](../providers/teams.md).

## <a name="properties"></a>Свойства

По умолчанию компонент `mgt-person` передает сведения о пользователе `mgt-person-card` компоненту. Однако эти атрибуты можно использовать для изменения такого поведения при создании шаблонов компонента `mgt-person` или при использовании компонента `mgt-person-card` в качестве отдельного компонента.

| Атрибут         | Тип                     | Описание                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Объект пользователя, определенный в Microsoft Graph и содержащий подробные сведения о пользователе. |
| person-image   | string                    | Универсальный код ресурса (URI) изображения, связанный с человеком, который отображается в карточке.                                   |
| inherit-details   | Отсутствует.                  | Разрешает проработку дерева родителей для компонента `mgt-person` для использования одинаковых данных `person-details` и `person-image`.                      |
| user-id | string | Позволяет разработчикам поставлять пользовательский id для получения данных, показанных на компоненте person-card |
| person-query | string | Позволяет разработчикам поставлять запрос пользователя для получения данных, показанных на компоненте person-card |


## <a name="templates"></a>Шаблоны

В компоненте Person-Card используются [шаблоны](../customize-components/templates.md), позволяющие добавлять и заменять части компонента. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| - | - | - |
| no-data | null | Шаблон, используемый, если данные недоступны.
| default | `person`: объект сведений о пользователе <br> `personImage`: URL-адрес изображения. | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |
| person-details | `person`: объект сведений о пользователе | Шаблон, используемый для отображения верхней части карточки пользователя. |
| additional-details | `person`: объект сведений о пользователе <br> `personImage`: URL-адрес изображения | Шаблон, который используется для добавления настраиваемого контента в контейнер дополнительных сведений. |

Например, шаблон можно использовать для настройки компонента, вложенного в компонент `mgt-person`, и шаблона, чтобы добавить дополнительные сведения в карточку. 

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

## <a name="events"></a>События

Из компонента инициируются следующие события.

| Событие | Описание |
| --- | --- |
| `expanded` | Пользователь открыл расширенный раздел сведений карты. |

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

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот элемент управления Person-Card использует следующие API и разрешения Microsoft Graph.

| Конфигурация | Разрешение | API | Section |
| --- | ---------- | ------- | --------- |
| `personDetails` установить с `id` пользователем, но без электронной почты, или `userId` установить, или `personQuery` установить `me` | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get) | По умолчанию |
| `personQuery` значение, отличаее от `me` | People.Read | [/me/people/?$search=](/graph/api/user-list-people) | По умолчанию |
| `personQuery` установлено значение, отличаее от значения `me` `config.useContactApis` `true` (по умолчанию) | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) | По умолчанию |
| `showPresence` установлено, что `true` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) | По умолчанию |
| `sections.organization` включено (по умолчанию) | User.Read.All | [/users/{id}/manager](/graph/api/user-list-manager) | Организация |
| `sections.organization.showWorksWith` set (по умолчанию) | People.Read.All | [/users/{id}/people](/graph/api/user-list-people) | Организация |
| `sections.mailMessages` включено (по умолчанию) | Mail.ReadBasic | [/me/messages](/graph/api/user-list-messages) | Сообщения |
| `sections.files` включено (по умолчанию) | Sites.Read.All | [/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used) | Файлы |

Класс `MgtPersonCard` также предоставляет `getScopes` статический метод, возвращающий массив областей, необходимый для работы карточки контакта с учетом глобальной конфигурации карточки контакта.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Проверка подлинности

В элементе управления Person-Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md). 

## <a name="cache"></a>Кэш

> [!IMPORTANT]
> Компонент `mgt-person-card` извлекает основные данные человека из родительского компонента, `mgt-person` не вызывая Graph. Когда используется отдельно, он извлекает необходимые данные и `mgt-person-card` кэширует их. Данные, отображаемые в разделах карты, извлекаются отдельно и не кэшются.

|Хранилище объектов|Кэшные данные|Примечания|
|---------|-----------|-------|
|`people`|Сведения о человеке|Используется при `personQuery` указании и его значение отличается от `me`|
|`photos`|Фотография человека|
|`presence`|Присутствие человека|Используется, `showPresence` когда установлено `true`|
|`users`|Сведения о пользователях|Используется при `userId` указании или `personQuery` задан `me`|

Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)
