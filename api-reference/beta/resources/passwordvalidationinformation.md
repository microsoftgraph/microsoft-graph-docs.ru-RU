---
title: тип ресурса passwordValidationInformation
description: Предоставляет свойства, которые указывают, допустим ли пароль пользователя при проверке в отношении политики проверки паролей клиента.
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 0da72df7551b84284dc9caa7d9183ef31834eba7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689367"
---
# <a name="passwordvalidationinformation-resource-type"></a>тип ресурса passwordValidationInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет свойства, которые указывают, допустим ли пароль пользователя, при проверке в отношении политики проверки паролей клиента. Этот ресурс также возвращает список правил, по которым был проверен пароль, и передает ли пароль пользователя эти роли.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isValid|Логический| Указывает, является ли пароль допустимым на основе расчета результатов в **свойстве validationResults.** Значение null не допускается. Только для чтения. |
|validationResults|[коллекция validationResult](../resources/validationresult.md)| Список правил проверки пароля и того, прошел ли пароль эти правила. Значение null не допускается. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordValidationInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordValidationInformation",
  "isValid": "Boolean",
  "validationResults": [
    {
      "@odata.type": "microsoft.graph.validationResult"
    }
  ]
}
```

