---
title: Тип ресурса validationResult
description: Предоставляет свойства, в которых указаны правила проверки пароля пользователя, а также результаты проверки.
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2e77770749ba06fed83e2855ff465922420da988
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689360"
---
# <a name="validationresult-resource-type"></a>Тип ресурса validationResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет свойства, в которых указаны правила проверки пароля пользователя, а также результаты проверки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|message|String| Строка, содержащая причину, по которой правило прошло или нет. Только для чтения. Значение null не допускается.|
|ruleName|String| Строка, содержащая имя правила проверки пароля, против которого было проверено действие. Только для чтения. Значение null не допускается.|
|validationPassed|Логический| Прошел ли пароль или не справился с правилом проверки. Только для чтения. Значение null не допускается.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.validationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.validationResult",
  "ruleName": "String",
  "validationPassed": "Boolean",
  "message": "String"
}
```

