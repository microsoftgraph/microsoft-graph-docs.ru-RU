---
title: Компонент person в microsoft Graph набор средств
description: Компонент person используется для отображения человека или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660041"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Компонент person в microsoft Graph набор средств

Компонент лица используется для отображения человека или контакта с помощью его фотографии, имени, адреса электронной почты или любых других сведений о человеке.

Компонент пользователя также использует [карточку mgt-person для](./person-card.md) отображения карточки с дополнительными сведениями о пользователе. Подробные сведения см. в [разделе "Карточка человека".](#person-card)

## <a name="example"></a>Пример

В следующем примере отображается человек, использующий `mgt-person` компонент. С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>Настройка сведений о человеке

Чтобы установить сведения о человеке, можно использовать три свойства. Используйте только одно из следующих свойств для каждого экземпляра:

* Установите атрибут или свойство для получения пользователя `user-id` из Microsoft Graph по его `userId` ИД.

* Установите атрибут `person-query` или свойство для поиска в Microsoft Graph для `personQuery` заданного человека. Он выберет первого доступного человека и получит сведения о нем. Сообщение электронной почты лучше всего работает для запроса нужного человека, но имя также работает.

* Установите атрибут `person-presence` или `personPresence` свойство, чтобы добавить эмблему присутствия для аватара пользователя вручную.

* Установите для `avatar-size` атрибута `avatarSize` или свойства или `small` `large` определите размер аватара. Это помогает добавить правильный [индикатор присутствия в](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) аватар. Вам потребуется выбрать правильные соответствующие настраиваемые свойства CSS, показанные ниже, чтобы дополнительно настроить размер аватара. По умолчанию устанавливается значение, которое автоматически определяет, как отрисовка присутствия на основе `auto` `view` свойства. Рекомендуется использовать, если размер вашего аватара меньше `small` 32px на 32px. 

* Используйте атрибут или свойство, чтобы вручную установить сведения о `person-details` `personDetails` человеке, как показано в следующем примере.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  Если изображение не предоставлено, он будет извлечен (если он доступен).

## <a name="properties"></a>Свойства

Для настройки компонента можно использовать несколько свойств.

| Атрибут       | Свойство       | Описание                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| user-id         | userId         | Установите для ид пользователя извлечение сведений и изображения этого пользователя из Microsoft Graph.|
| person-query    | personQuery    | Запишите имя или сообщение электронной почты человека для поиска человека в Microsoft Graph и получения сведений и изображения первого человека.|
| person-details  | personDetails  | Установите объект, представляющий человека. Работает с объектом из людей, пользователей, контактов или групп, ресурсов. |
| person-image    | personImage    | Закажите изображение, которое будет показываться для этого человека. |
| person-presence | personPresence | Установите присутствие для человека. |
| fetch-image     | fetchImage     | Установите флаг для автоматического извлечения из Microsoft Graph на основе `personImage` `personDetails` объекта, предоставленного пользователем. |
| view            | view           | Установите для управления отрисовки человека. Значение по умолчанию: `avatar` <br /> `avatar` — показывать только аватар <br /> `oneline` - показать аватар и первую строку ( `displayName` по умолчанию) <br /> `twolines` - показать аватар и две строки текста ( `displayName` и `mail` по умолчанию)|
| line1-property  | line1Property  | Задает свойство personDetails, используемого для первой строки текста. Значение по умолчанию: `displayName`.|
| line2-property  | line2Property  | Задает свойство personDetails, используемого для второй строки текста. Значение по умолчанию: `mail`.|
| line3-property  | line3Property  | Задает свойство personDetails, используемого для третьей строки текста. Значение по умолчанию: `jobTitle`.|
| show-presence   | showPresence   | Установите флаг для отображения присутствия человека — значение по `false` умолчанию.|

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

Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)

## <a name="templates"></a>Шаблоны

Компонент `mgt-person` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента. Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:

| Тип данных | Контекст данных | Описание |
| --------- | ------------ | ----------- |
| loading | Нет | Шаблон для отрисовки, когда компонент находится в состоянии загрузки. |
| no-data | Нет | Шаблон, который необходимо отрисовки, если изображение или данные человека недоступны. | 
| default | person: объект сведений о человеке <br> `personImage`: URL-адрес изображения | Шаблон по умолчанию заменяет весь компонент на собственный. |
| person-card | person: объект сведений о человеке <br> `personImage`: URL-адрес изображения | Шаблон для обновления карточки mgt-person, отображаемой при наведении или щелчке. |

В следующем примере определяется шаблон для компонента person.

```html
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
```

## <a name="person-card"></a>Карточка человека

Компонент `mgt-person` может показываться при `mgt-person-card` наведении или нажатии кнопки мыши.

### <a name="add-the-control-to-the-html-page"></a>Добавление элементов управления на HTML-страницу
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Атрибут    |  Свойство     | Описание                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | Enumeration to determine user action necessary to activate flyout panel - `hover` or `click` . Значение по умолчанию: `none` |


Дополнительные сведения о шаблонах, стилях и атрибутах см. в компоненте [карточки человека.](./person-card.md)

## <a name="global-component-configuration"></a>Глобальная конфигурация компонентов

Класс `MgtPerson` предоставляет статический `config` объект, который настраивает все компоненты person в приложении.

В следующем примере показано, как использовать объект config.

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

Для объекта config доступны следующие свойства.

| Свойство | Описание |
| ------------ | ------------- |
| useContactApis | `boolean` - Указывает, может ли компонент лица использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий. Значение по умолчанию: `true`.  |

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот контроль использует следующие API Microsoft Graph и разрешения.

| Ресурс | Разрешение     |
| -| - |
| [/me](/graph/api/user-get)                              | User.Read          |
| [/me/photo/$value](/graph/api/profilephoto-get)        | User.Read          |
| [/me/people/?$search=](/graph/api/user-list-people)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get)        | Presence.Read.All |

## <a name="authentication"></a>Проверка подлинности

Для получения необходимых данных этот контроль [](../providers/providers.md) использует глобального поставщика проверки подлинности, описанного в документации по проверке подлинности.

## <a name="extend-for-more-control"></a>Расширение для большего контроля

Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.

| Метод | Описание |
| - | - |
| renderLoading | Отрисовка состояния загрузки. |
| renderNoData | Отрисовка, когда данные изображения или человека недоступны. |
| renderAvatar | Отрисовка аватара. |
| renderDetails | Отрисовка части сведений о человеке. |
