---
title: Тип ресурса submissionAdminReview
description: Представляет сведения о проверке администратором для отправки угроз
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 410ffc88cb5d5fade44456b928996834c7722cac
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856849"
---
# <a name="submissionadminreview-resource-type"></a>Тип ресурса submissionAdminReview

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о проверке администратором для отправки угрозы. В настоящее время поддерживается только отправка сообщений электронной почты с сообщением об угрозах, о которых сообщил пользователь, и их может просмотреть администратор.

## <a name="properties"></a>Свойства
| Свойство       | Тип                     | Описание                                  |
|:---------------|:-------------------------|:---------------------------------------------|
| reviewBy       | Строка                   | Указывает, кто просматривал сообщение электронной почты. Идентификация — это идентификатор электронной почты или другие строки удостоверения.|
| reviewDateTime | DateTimeOffset           | Указывает дату, когда была выполнена проверка.|
| reviewResult   | submissionResultCategory | Указывает результат проверки. Возможные значения: `notJunk`, , `spam`, `phishing`, `malware`, `allowedByPolicy`, `blockedByPolicy`, `spoof`, `unknown`и `noResultAvailable``unknownFutureValue`.  |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionAdminReview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionAdminReview",
  "reviewDateTime": "String (timestamp)",
  "reviewResult": "String",
  "reviewBy": "String"
}
```

