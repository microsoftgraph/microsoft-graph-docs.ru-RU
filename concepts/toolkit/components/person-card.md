---
title: Компонент Person Card в наборе инструментов Microsoft Graph
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: f4d8c975fe91d91658f512cea708ee104d4fd906
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275859"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Компонент Person Card в наборе инструментов Microsoft Graph

Компонент Person-Card — это реагирующий на работу компонент для отображения дополнительных сведений, относящихся к пользователю. Он обычно используется в качестве всплывающего элемента в `mgt-person` компоненте.

Дополнительную информацию о компоненте `mgt-person` можно узнать в статье [упр](./person.md).
  
## <a name="example"></a>Пример

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a>Свойства

Компонент использует Microsoft Graph для предоставления дополнительных сведений о пользователе. Чтобы определить пользователя, необходимо использовать свойство **Person — запрос** `mgt-person`.

| Атрибут         | type                     | Описание                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| Person — сведения | MicrosoftGraph. User <br> MicrosoftGraph. Person <br> MicrosoftGraph. Contact | Объект Person, определенный Microsoft Graph, содержащий сведения, связанные с пользователем. |
| Person — изображение   | PNG/JPG/SVG                    | Изображение, связанное с лицом, которое отображается в карточке.                                   |



## <a name="templates"></a>Шаблоны

Компонент Person Card использует [шаблоны](../templates.md) , позволяющие добавлять или заменять части компонента. Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| умолчани | Person: объект сведений о лице <br> Персонимаже: URL-адрес изображения | Шаблон по умолчанию заменяет весь компонент своим собственным. |
| Дополнительные сведения | Person: объект сведений о лице <br> Персонимаже: URL-адрес изображения | Шаблон, используемый для добавления в карточку дополнительного контента. |

Например, вы можете использовать шаблон для настройки компонента, присоединенного к `mgt-person` компоненту, и шаблона, чтобы добавить дополнительные сведения в карточку. 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card person-details="{{person}}" 
            person-image="{{personImage}}">
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

`mgt-person-card` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений. 

## <a name="authentication"></a>Проверка подлинности

В элементе управления Person Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md). 
