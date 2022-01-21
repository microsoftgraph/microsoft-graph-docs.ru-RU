---
title: Тип ресурса authenticationContext
description: Описывает контекст проверки подлинности условного доступа для события входного знака.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c768615d585423f2dd99c95961965d415bde1244
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137270"
---
# <a name="authenticationcontext-resource-type"></a>Тип ресурса authenticationContext

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает контекст проверки подлинности условного доступа для события входного знака. 

Дополнительные сведения о контексте проверки подлинности в условном доступе см. в документации по [контексту условного доступа.](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#authentication-context-preview) 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подробные|authenticationContextDetail|Описывает, как был вызван контекст проверки подлинности условного доступа. Значение контекста auth было потому, что пользователь уже удовлетворил требования к этому контексту проверки подлинности в некоторых предыдущих событиях проверки `previouslySatisfied` подлинности. Значение средств, необходимых пользователю для удовлетворения требования контекста проверки подлинности в рамках потока `required` регистрации. Допустимые значения: `required`, `previouslySatisfied`, `notApplicable`, `unknownFutureValue`.|
|id|Строка|Идентификатор контекста проверки подлинности в клиенте.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationContext"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationContext",
  "id": "String (identifier)",
  "detail": "String"
}
```

