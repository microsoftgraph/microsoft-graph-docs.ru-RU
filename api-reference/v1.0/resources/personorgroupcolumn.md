---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.localizationpriority: medium
ms.prod: insights
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
doc_type: resourcePageType
ms.openlocfilehash: dd349e34fa08ecce8761e12bb50b45612bf00dcf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117796"
---
# <a name="personorgroupcolumn-resource-type"></a>Тип ресурса personOrGroupColumn

Пространство имен: microsoft.graph

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

## <a name="displayas-options"></a>Параметры DisplayAs

| Значение DisplayAs               | Описание
|:------------------------------|:-----------------------
| **account**                   | Необработанная закодированная строка утверждения SharePoint для человека или группы (например, `i:0#.f|membership|jane@contoso.com`).
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->

