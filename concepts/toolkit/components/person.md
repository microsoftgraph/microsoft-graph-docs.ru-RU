---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b4664cf545c858dbb2d49ad5191ab7cf5118092e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275705"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Компонент Person в наборе инструментов Microsoft Graph

Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты. 

Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person. Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .

## <a name="example"></a>Пример

[Пример жсфиддле](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a>Добавление элемента управления на HTML-страницу
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a>Настройка сведений о лице

Для задания сведений о лице можно использовать три свойства. Используйте только одно из следующих свойств для каждого экземпляра:

* Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.  

* Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph. Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице. Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.

* Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  Если изображение не указано, выбирается один из них (если он доступен).

## <a name="changing-how-the-component-looks"></a>Изменение вида компонента

Для настройки компонента можно использовать несколько свойств.

| Свойство    | Атрибут    | Описание                                                   |
| ----------- | ------------ | ------------------------------------------------------------- |
| шовнаме  | Show (имя)  | Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —. |
| шовемаил | Show — email | Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.        |

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).

## <a name="templates"></a>Шаблоны

`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента. Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:

| Тип данных     | Контекст данных              | Описание                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| умолчани     | Person: объект сведений о лице <br> `personImage`: URL-адрес изображения | Шаблон по умолчанию заменяет весь компонент своим собственным. |
| Person — карточка | Person: объект сведений о лице <br> `personImage`: URL-адрес изображения | Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью. |

В следующем примере определяется шаблон для компонента Person.

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>Карточка лица

`mgt-person` Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.

### <a name="add-the-control-to-the-html-page"></a>Добавление элемента управления на HTML-страницу
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Свойство     | Атрибут     | Описание                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| персонкард | Person — карточка | Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели. Значение по умолчанию:`none` |


Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.

| Ресурс                                                                                                    | Разрешение     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/ме](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [/ме/фото/$value](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/ме/Пеопле/? $search =](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/ме/контактс/*](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [/усерс/{ИД}/фото/$value](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |

> **Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.

## <a name="authentication"></a>Проверка подлинности

Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .
