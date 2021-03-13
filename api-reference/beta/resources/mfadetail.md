---
title: тип ресурса mfaDetail
description: 'Указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: телефон, SMS или голосовая почта) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b3cd2392b9591cfb5465f2f269db547cd37754ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759799"
---
# <a name="mfadetail-resource-type"></a>тип ресурса mfaDetail

Пространство имен: microsoft.graph указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: телефон, SMS или голосовая почта)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|authDetail|String|Указывает подробную информацию об auth MFA для соответствующей активности регистрации, когда требуется MFA является "Да".|
|authMethod|String|Указывает, что методы auth MFA (SMS, Phone, Authenticator App являются некоторыми из значений) для соответствующей активности входных данных, когда поле MFA Обязательное "Да".|

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


