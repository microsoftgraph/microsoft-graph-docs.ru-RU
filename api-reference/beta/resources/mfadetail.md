---
title: Тип ресурса Мфадетаил
description: 'Указывает сведения о MFA для определенного входа. Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте). '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: besiler
ms.openlocfilehash: 97e075d6f12c102d366f63fd231d83c1144d16f3
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524549"
---
# <a name="mfadetail-resource-type"></a>Тип ресурса Мфадетаил

Пространство имен: Microsoft. Graph указывает сведения о MFA для определенного входа. Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте).



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|аусдетаил|String|Указывает сведения о проверке подлинности MFA для соответствующего действия при входе, если для MFA необходимо значение "Да".|
|аусмесод|String|Указывает методы проверки подлинности MFA (SMS, Phone, приложение проверки подлинности — это часть значения) для соответствующего действия входа, если поле "обязательное MFA" имеет значение "Да".|

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


