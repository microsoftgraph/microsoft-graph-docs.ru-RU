---
title: Тип ресурса fileUrlThreatSubmission
description: Представляет объект отправки угрозы файла, созданный при отправке с использованием URL-адреса файла.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b77f0fd8e8fb962546cd473bd3159ae7901c054c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856903"
---
# <a name="fileurlthreatsubmission-resource-type"></a>Тип ресурса fileUrlThreatSubmission

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект отправки угрозы файла, созданный при отправке с использованием URL-адреса файла. Этот API зарезервирован и в настоящее время не поддерживается.

Наследуется [от fileThreatSubmission](../resources/security-filethreatsubmission.md).

## <a name="properties"></a>Свойства
| Свойство | Тип   | Описание                   |
|:---------|:-------|:------------------------------|
| fileUrl  | Строка | Он указывает URL-адрес файла, который необходимо отправить. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileUrlThreatSubmission",
  "baseType": "microsoft.graph.security.fileThreatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileUrlThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "fileName": "String",
  "fileUrl": "String"
}
```

