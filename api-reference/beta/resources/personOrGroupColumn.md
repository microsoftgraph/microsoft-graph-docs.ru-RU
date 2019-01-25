---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519299"
---
# <a name="personorgroupcolumn-resource-type"></a>Тип ресурса personOrGroupColumn

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

## <a name="displayas-values"></a>Значения DisplayAs

| Значение DisplayAs               | Описание
|:------------------------------|:-----------------------
| **account**                   | Необработанная закодированная строка утверждения SharePoint для человека или группы (например, i:0#.f|membership|olga@contoso.com).
| **department**                | Отдел человека или группы.
| **firstName**                 | Имя человека.
| **id**                        | Идентификатор человека или группы в каталоге.
| **lastName**                  | Фамилия человека.
| **mobilePhone**               | Номер мобильного телефона человека.
| **name**                      | Имя человека.
| **nameWithPictureAndDetails** | Имя человека, а также его изображение и дополнительные сведения о нем.
| **nameWithPresence**          | Значение, используемое по умолчанию. Имя человека со значком индикатора присутствия (доступен, занят и т. д.)
| **office**                    | Номер офиса человека.
| **pictureOnly36x36**          | Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.
| **pictureOnly48x48**          | Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.
| **pictureOnly72x72**          | Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.
| **sipAddress**                | SIP-адрес человека.
| **title**                     | Должность человека в организации.
| **userName**                  | Имя пользователя человека или группы.
| **workEmail**                 | Электронный адрес человека или группы.
| **workPhone**                 | Номер рабочего телефона человека.

Примечание. Система может возвращать дополнительные типы DisplayAs.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
