---
title: тип ресурса mfaDetail
description: 'Указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: Телефон, SMS или голосовая почта) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: 52cf5f15c31502fd796e581f8b45e8d00b80eeb83939d7bb6b3c70d6c4906ef2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249701"
---
# <a name="mfadetail-resource-type"></a>тип ресурса mfaDetail

Пространство имен: microsoft.graph указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: Телефон, SMS или голосовая почта)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|authDetail|String|Указывает подробную информацию об auth MFA для соответствующей активности регистрации, когда требуется MFA является "Да".|
|authMethod|Строка|Указывает, что методы auth MFA (SMS, Телефон, Authenticator App являются одними из значений) для соответствующей активности регистрации, когда поле MFA Обязательное "Да".|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


