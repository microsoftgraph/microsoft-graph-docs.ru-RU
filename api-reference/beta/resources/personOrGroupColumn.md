---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 261ed729bc865b6679bf6dc9d08060148f32006a
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176411"
---
# <a name="personorgroupcolumn-resource-type"></a>Тип ресурса personOrGroupColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a>Свойства

| Имя свойства              | Тип    | Описание
|:---------------------------|:--------|:--------------------------------------
| **allowMultipleSelection** | boolean | Указывает, можно ли выбрать несколько значений в источнике.
| **displayAs**              | string  | Указывает способ отображения сведений о выбранном человеке или группе. См. ниже.
| **chooseFromType**         | string  | Указывает, что можно выбирать: только людей либо людей и группы. Должно иметь тип `peopleAndGroups` или `peopleOnly`.

## <a name="displayas-values"></a>Значения displayAs

| Значение               | Описание                                                                                                 |
|:------------------------------|:------------------------------------------------------------------------------------------------------------|
| **account**                   | Необработанная закодированная строка утверждения SharePoint для человека или группы (например, `i:0#.f|membership|jane@contoso.com`). |
| **department**                | Отдел человека или группы.                                                                           |
| **firstName**                 | Имя человека.                                                                                    |
| **id**                        | Идентификатор человека или группы в каталоге.                                                             |
| **lastName**                  | Фамилия человека.                                                                                     |
| **mobilePhone**               | Номер мобильного телефона человека.                                                                           |
| **name**                      | Имя человека.                                                                                          |
| **nameWithPictureAndDetails** | Имя человека, а также его изображение и дополнительные сведения о нем.                                          |
| **nameWithPresence**          | Значение, используемое по умолчанию. Имя человека со значком индикатора присутствия (доступен, занят и т. д.)                             |
| **office**                    | Номер офиса человека.                                                                                 |
| **pictureOnly36x36**          | Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.                                                         |
| **pictureOnly48x48**          | Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.                                                         |
| **pictureOnly72x72**          | Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.                                                         |
| **sipAddress**                | SIP-адрес человека.                                                                                   |
| **title**                     | Должность человека в организации.                                                                     |
| **userName**                  | Имя пользователя человека или группы.                                                                            |
| **workEmail**                 | Электронный адрес человека или группы.                                                                        |
| **workPhone**                 | Номер рабочего телефона человека.                                                                             |

Примечание. Система может возвращать дополнительные типы DisplayAs.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->


