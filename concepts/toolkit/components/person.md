---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 3d69bddd473bf43de4d713207ab8f54291cbcd7f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589039"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Компонент пользователя в Microsoft Graph Toolkit

Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, адреса электронной почты и любых других сведений о пользователе.

Кроме того, в компоненте пользователя используется [mgt-person-card](./person-card.md) для отображения карточки всплывающего окна с дополнительной информации о пользователе. Дополнительные сведения см. в разделе [Карточка пользователя](#person-card).

## <a name="example"></a>Пример

В приведенном далее примере показан пользователь, использующий компонент `mgt-person`. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>Настройка сведений о пользователе

Чтобы задать сведения о пользователе, можно использовать три свойства. Используйте только одно из указанных далее свойств для одного случая:

* Задайте атрибут `user-id` или свойство `userId`, чтобы получить данные пользователя из Microsoft Graph, используя его идентификатор.

* Чтобы выполнить поиск определенного пользователя в Microsoft Graph, задайте атрибут `person-query` или свойство `personQuery`. При этом будет выбран первый доступный пользователь и будут получены сведения об этом пользователе. Электронная почта лучше всего подходит для того, чтобы найти нужного пользователя, но можно использовать и имя.

* Задайте атрибут `person-presence` или свойство `personPresence`, чтобы добавить значок присутствия в аватар пользователя вручную.

* Чтобы определить размер аватара, задайте для атрибута `avatar-size` или свойства `avatarSize` значение `small` или `large`. Это позволяет добавить [правильный значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в аватар. Чтобы дополнительно настроить размер аватара, вам нужно выбрать соответствующие настраиваемые свойства CSS, указанные далее. Для этого параметра по умолчанию задано значение `auto`, благодаря которому присутствие будет обрабатываться автоматически с учетом свойства `view`. Рекомендуем использовать `small`, если аватар меньше 32 на 32 пикс. 

* Чтобы вручную задать сведения о пользователе, используйте атрибут `person-details` или свойство `personDetails`, как показано в приведенном далее примере.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  Если изображение не предоставлено, оно будет получено (при наличии).

* По умолчанию компонент пользователя запрашивает только стандартный набор свойств Graph [Майкрософт.](/graph/api/user-get?&tabs=http#optional-query-parameters) Чтобы запросить дополнительные свойства, объявите их в качестве любой части `line(x)Property`. 


## <a name="properties"></a>Свойства

Для настройки компонента можно использовать несколько свойств.

| Атрибут       | Свойство       | Описание                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| user-id         | userId         | Установите идентификатор пользователя, чтобы получить сведения об этом пользователе и его изображение из Microsoft Graph.|
| person-query    | personQuery    | Чтобы найти пользователя в Microsoft Graph, установите его имя или адрес электронной почты пользователя и получите сведения о первом пользователе и его изображение.|
| person-details  | personDetails  | Установите объект, представляющий пользователя. Используется для объекта из ресурсов "люди", "пользователи", "контакты" или "группа". |
| fallback-details| fallbackDetails| Установите объект, представляющий человека, если в графе не обнаружено пользователя/пользователя/контакта.
| person-image    | personImage    | Задать изображение, которое будет отображаться для пользователя. |
| person-presence | personPresence | Установка присутствия для пользователя. |
| fetch-image     | fetchImage     | Установите флажок для автоматического получения `personImage` из Microsoft Graph на основе объекта `personDetails`, предоставленного пользователем. |
| отключение-извлечение изображений | disableImageFetch | Установите флаг, чтобы отключить извлечение изображения человека. Можно использовать, чтобы избежать ненужных извлечений из Microsoft Graph при указании `personImage` свойства.
| тип аватара     | avatarType     | Установите или `initials` отобразить `photo` состояние отображения по умолчанию — это фотография. |
| представление            | представление           | Установите, чтобы настроить, как выглядит пользователь. Значение по умолчанию: `avatar` <br /> `avatar` — Показывать только аватар <br /> `oneline` — Показывать аватар и первую строку (`displayName` по умолчанию) <br /> `twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию) <br /> `threelines` - показать аватар и три строки текста (`displayName`и `mail` по `jobTitle` умолчанию) |
| line1-property  | line1Property  | Задает свойство personDetails для использования для первой строки текста. Значение по умолчанию: `displayName`.|
| line2-property  | line2Property  | Задает свойство personDetails для использования для второй строки текста. Значение по умолчанию: `mail`.|
| line3-property  | line3Property  | Задает свойство personDetails для использования для третьей строки текста. Значение по умолчанию: `jobTitle`.|
| show-presence   | showPresence   | Установить флажок отображения присутствия пользователя — по умолчанию `false`.|

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="events"></a>События

Из компонента инициируются следующие события.

Событие | Когда он излучается | Настраиваемые данные | Отмена | Пузыри | Работает с настраиваемой шаблонной
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`line1clicked` | Увольнение при нажатии строки1 | Объект`person`, который может быть Graph [пользователем](/graph/api/resources/user)[](/graph/api/resources/contact)[,](/graph/api/resources/person) `personImage` лицом или контактом с дополнительным свойством, содержаным URL-адрес фотографии пользователя | Нет | Нет | Да, если не переопределить шаблон по умолчанию
`line2clicked` | Увольнение при нажатии строки2 | Объект`person`, который может быть Graph [пользователем](/graph/api/resources/user)[](/graph/api/resources/contact)[,](/graph/api/resources/person) `personImage` лицом или контактом с дополнительным свойством, содержаным URL-адрес фотографии пользователя | Нет | Нет | Да, если не переопределить шаблон по умолчанию
`line3clicked` | Увольнение при нажатии строки 3 | Объект`person`, который может быть Graph [пользователем](/graph/api/resources/user)[](/graph/api/resources/contact)[,](/graph/api/resources/person) `personImage` лицом или контактом с дополнительным свойством, содержаным URL-адрес фотографии пользователя | Нет | Нет | Да, если не переопределить шаблон по умолчанию

Дополнительные сведения об обработке событий см. в [этой информации](../customize-components/events.md).

## <a name="templates"></a>Шаблоны

Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --------- | ------------ | ----------- |
| загрузка | Нет | Шаблон для отображения состояния загрузки компонента. |
| no-data | Нет | Шаблон для использования, если изображения или данные не доступны. | 
| default | пользователь: объект сведений о пользователе <br> `personImage`: URL-адрес изображения. <br> `personPresence`: Объект сведений о присутствии для человека  | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |
| person-card | пользователь: объект сведений о пользователе <br> `personImage`: URL-адрес изображения. | Шаблон для обновления карточки mgt-person-card, отображаемой при наведении указателя мыши или щелчке мышью. |
| line1 | person: объект сведений о пользователе | Шаблон для первой строки метаданных человека. |
| line2 | person: объект сведений о пользователе | Шаблон для второй строки метаданных человека. |
| line3 | person: объект сведений о пользователе | Шаблон для третьей строки метаданных человека. |

В следующем примере определяется шаблон для компонента пользователя.

```html
<!-- Retemplate the entire person component -->
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>Карточка пользователя

`mgt-person` Компонент может отображаться`mgt-person-card` при либо наведении указателя мыши, либо щелчка мышью.

### <a name="add-the-control-to-the-html-page"></a>Добавьте средство управления на HTML-страницу.
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Атрибут    |  Свойство     | Описание                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`. Значение по умолчанию: `none`. |


Дополнительные сведения о шаблонах, стилях и атрибутах см. в статье [Компонент карточки пользователя](./person-card.md).

## <a name="global-component-configuration"></a>Конфигурация глобального компонента

Класс `MgtPerson` предоставляет статический объект `config`, который конфигурирует все компоненты пользователя в приложении.

В приведенном ниже примере показано, как использовать объект конфигурации.

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

Ниже указаны свойства, доступные в объекте конфигурации.

| Свойство | Описание |
| ------------ | ------------- |
| useContactApis | `boolean` — Указывает, может ли компонент пользователя использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий. Значение по умолчанию: `true`.  |

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот элемент управления использует следующие API и разрешения Microsoft Graph.

| Конфигурация | Разрешение | API |
| ------------- | ---------- | --- |
| `personDetails` установить без изображения, `fetchImage` установить `true`, установить `avatarType` `photo`, извлекаемого человека является контакт и `useContactApis` установить `true` | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `personDetails` установить без изображения, `fetchImage` установить `true`, `avatarType` установить `photo` и лицо не является контактом или `useContactApis` установлено, чтобы `false` | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` набор без изображения, `fetchImage` установленный `true`для , заданный `avatarType` `photo` пользователем и указанный по электронной почте | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` набор без изображения, `fetchImage` заданный `true`, заданный `avatarType` `photo` и контакт, указанный по электронной почте | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `userId` set | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people) |
| `personQuery` установлено и `me` `avatarType` установлено `photo` | User.Read | [/ме/фото/$value](/graph/api/profilephoto-get) |
| `personQuery` установлено и `me` установлено `avatarType` что-то другое, чем `photo` | User.Read | [/me](/graph/api/user-get) |
| `personQuery`значение, заме-`me` `useContactApis``true` | People.Read, User.ReadBasic.All, Contacts.Read | [/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts) |
| `personQuery`значение, заме-`me` `useContactApis``false` | People.Read, User.ReadBasic.All | [/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people) |
| `showPresence` установлено и `true` `personQuery` установлено `me` | Presence.Read | [/me/presence](/graph/api/presence-get) |
| `showPresence` установлено `true` значение `personQuery` , заме- `me` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) |
| `personCardInteraction` значение, заме- `PersonCardInteraction.none` | См [. разрешения на карточку человека](/graph/toolkit/components/person-card#microsoft-graph-permissions) | См [. вызовы API карт персоны](/graph/toolkit/components/person-card#microsoft-graph-permissions) |

## <a name="authentication"></a>Проверка подлинности

Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

|Хранилище объектов|Кэшные данные|Примечания|
|---------|-----------|-------|
|`photos`|Фотография человека|Используется, когда `avatarType` установлено `photo` `fetchImage` и установлено `true`|
|`presence`|Присутствие человека|Используется, когда `showPresence` установлено `true`|
|`users`|Сведения о пользователях|

Дополнительные сведения о настройке кэша см. в [caching](../customize-components/cache.md) .

## <a name="extend-for-more-control"></a>Расширение для дополнительного управления

В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.

| Метод | Описание |
| - | - |
| renderLoading | Отображает состояние загрузки. |
| renderNoData | Отображается, если изображение или данные о пользователе недоступны. |
| renderAvatar | Отображает аватар. |
| renderDetails | Отображает сведения о пользователе. |
