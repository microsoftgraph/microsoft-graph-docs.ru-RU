---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9ac8eebfaa4d95ccd935414329ab1dd145839dd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475060"
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
| тип аватара     | avatarType     | Установите или `initials` `photo` отобразить состояние отображения по умолчанию — это фотография. |
| представление            | представление           | Установите, чтобы настроить, как выглядит пользователь. Значение по умолчанию: `avatar` <br /> `avatar` — Показывать только аватар <br /> `oneline` — Показывать аватар и первую строку (`displayName` по умолчанию) <br /> `twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию)|
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

| Событие | Сведения | Описание |
| --- | --- | --- |
| line1clicked | Сведения содержат соответствующий объект `person` | Уволено при нажатии строки 1. |
| line2clicked | Сведения содержат соответствующий объект `person` | Уволено при нажатии строки2. |
| line3clicked | Сведения содержат соответствующий объект `person` | Уволено при нажатии строки 3. |

## <a name="templates"></a>Шаблоны

Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --------- | ------------ | ----------- |
| загрузка | Нет | Шаблон для отображения состояния загрузки компонента. |
| no-data | Нет | Шаблон для использования, если изображения или данные не доступны. | 
| default | пользователь: объект сведений о пользователе <br> `personImage`: URL-адрес изображения. | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |
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

| Ресурс | Разрешение     |
| -| - |
| [/me](/graph/api/user-get)                              | User.Read          |
| [/ме/фото/$value](/graph/api/profilephoto-get)        | User.Read          |
| [/me/people/?$search=](/graph/api/user-list-people)     | People.Read        |
| [me/contacts\*](/graph/api/user-list-contacts&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get)        | Presence.Read.All |

## <a name="authentication"></a>Проверка подлинности

Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="extend-for-more-control"></a>Расширение для дополнительного управления

В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.

| Метод | Описание |
| - | - |
| renderLoading | Отображает состояние загрузки. |
| renderNoData | Отображается, если изображение или данные о пользователе недоступны. |
| renderAvatar | Отображает аватар. |
| renderDetails | Отображает сведения о пользователе. |
