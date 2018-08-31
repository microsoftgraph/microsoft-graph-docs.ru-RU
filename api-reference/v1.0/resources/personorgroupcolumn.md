---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 37c324ddb1863e3e589e7d17ea60bd879e50771f
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267558"
---
# <a name="personorgroupcolumn-resource-type"></a>Тип ресурса personOrGroupColumn

Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.

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
| **allowMultipleSelection** | логический | Указывает, можно ли выбрать несколько значений в источнике.
| **displayAs**              | строка  | Указывает способ отображения сведений о выбранном человеке или группе. См. ниже.
| **chooseFromType**         | строка  | Указывает, что можно выбирать: только людей либо людей и группы. Должно иметь тип `peopleAndGroups` или `peopleOnly`.

## <a name="displayas-options"></a>Параметры displayAs

| Значение DisplayAs               | Описание
|:------------------------------|:-----------------------
| **учетная запись**                   | Необработанная закодированная строка утверждения SharePoint для человека или группы (например, i:0#.f|членство|olga@contoso.com).
| **отдел**                | Отдел человека или группы.
| **firstName**                 | Имя человека.
| **ИД**                        | Идентификатор человека или группы в каталоге.
| **lastName**                  | Фамилия человека.
| **mobilePhone**               | Номер мобильного телефона человека.
| **имя**                      | Имя человека.
| **nameWithPictureAndDetails** | Имя человека, а также его изображение и дополнительные сведения о нем.
| **nameWithPresence**          | Значение, используемое по умолчанию. Имя человека со значком индикатора присутствия (доступен, занят и т. д.)
| **офис**                    | Номер офиса человека.
| **pictureOnly36x36**          | Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.
| **pictureOnly48x48**          | Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.
| **pictureOnly72x72**          | Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.
| **sipAddress**                | SIP-адрес человека.
| **должность**                     | Должность человека в организации.
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
