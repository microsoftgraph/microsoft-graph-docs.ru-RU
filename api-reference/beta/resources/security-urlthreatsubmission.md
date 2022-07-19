---
title: Тип ресурса urlThreatSubmission
description: Представляет отправку угрозы, связанную с URL-адресом
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f04e14d1482a935868f4a0a7985b43b6faf5188
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856884"
---
# <a name="urlthreatsubmission-resource-type"></a>Тип ресурса urlThreatSubmission

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отправку угрозы, связанную с URL-адресом.

Этот ресурс используется для отправки подозрительных URL-адресов фишинга в Microsoft Defender для Office 365. Его также можно использовать для отправки ложноположительных случаев, которые не должны быть заблокированы, например безопасных URL-адресов.

Наследуется [от threatSubmission](../resources/security-threatsubmission.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление urlThreatSubmissions](../api/security-urlthreatsubmission-list.md)|[Коллекция microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Получение списка объектов [urlThreatSubmission](../resources/security-urlthreatsubmission.md) и их свойств.|
|[Создание urlThreatSubmission](../api/security-urlthreatsubmission-post-urlthreats.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Создайте объект [urlThreatSubmission](../resources/security-urlthreatsubmission.md) .|
|[Получение urlThreatSubmission](../api/security-urlthreatsubmission-get.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Чтение свойств и связей объекта [urlThreatSubmission](../resources/security-urlthreatsubmission.md) .|

## <a name="properties"></a>Свойства
| Свойство | Тип   | Описание                 |
|:---------|:-------|:----------------------------|
| webUrl   | String | Обозначает webUrl, который необходимо отправить. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.urlThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.urlThreatSubmission",
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
  "webUrl": "String"
}
```

