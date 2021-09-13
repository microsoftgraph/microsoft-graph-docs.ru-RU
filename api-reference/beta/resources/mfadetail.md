---
title: тип ресурса mfaDetail
description: 'Указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: Телефон, SMS или голосовая почта) '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: 52ad666182e1ab404ba611e4ca2668745a8539fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100710"
---
# <a name="mfadetail-resource-type"></a>тип ресурса mfaDetail

Пространство имен: microsoft.graph указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: Телефон, SMS или голосовая почта)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|authDetail|String|Указывает подробную информацию об auth MFA для соответствующей активности регистрации, когда требуется MFA является "Да".|
|authMethod|String|Указывает, что методы auth MFA (SMS, Телефон, Authenticator App являются одними из значений) для соответствующей активности регистрации, когда поле MFA Обязательное "Да".|

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


