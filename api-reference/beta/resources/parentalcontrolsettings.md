---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643005"
---
# <a name="parentalcontrolsettings-resource-type"></a>Тип ресурса parentalControlSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметры родительского контроля для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция String| Указывает [двухбуквенный код страны ISO](https://www.iso.org/iso-3166-country-codes.html). Доступ к приложению будут блокироваться для минорам из указанной в этом списке.|
|legalAgeGroupRule| String | Правило срок хранения в юридическом группы, которая применяется для пользователей приложения. Может быть установлено одно из следующих значений: <table><tr><th>Значение</th><th>Описание</th></tr><tr><td>Allow (разрешить)</td><td>Значение, используемое по умолчанию. Требуют соблюдения юридических по меньшей мере. Это означает, что является обязательным для минорам в Европейском союзе и Корея, родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Обеспечивает пользователю для указания Дата рождения в соответствии с правилами COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для возраста ниже 18, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для возраста ниже 14, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>BlockMinors</td><td>Блоки минорам с помощью приложения.</td></tr></table> |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
