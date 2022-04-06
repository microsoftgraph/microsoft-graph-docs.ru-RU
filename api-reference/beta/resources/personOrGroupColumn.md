---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2e35c461dcec7cac70af8b6591a4fcb251ccc8e2
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720815"
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

| Свойство                   | Тип    | Описание                                                                                                        |
| :------------------------- | :------ | :----------------------------------------------------------------------------------------------------------------- |
| **allowMultipleSelection** | boolean | Указывает, можно ли выбрать несколько значений в источнике.                                                 |
| **displayAs**              | string  | Указывает способ отображения сведений о выбранном человеке или группе. См. ниже.                                        |
| **chooseFromType**         | string  | Указывает, что можно выбирать: только людей либо людей и группы. Должно иметь тип `peopleAndGroups` или `peopleOnly`. |

## <a name="displayas-values"></a>DisplayAs values

| Значение                         | Описание                                                                                                 |
| :---------------------------- | :---------------------------------------------------------------------------------------------------------- |
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
