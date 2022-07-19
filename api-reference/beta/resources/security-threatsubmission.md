---
title: Тип ресурса threatSubmission
description: Представляет отправку угроз, которая используется для отправки подозрительных угроз электронной почты, срока жизни или файлов в Microsoft Defender.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23651a4b66c68ce1c8d128268dd786dfcf667cf8
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856843"
---
# <a name="threatsubmission-resource-type"></a>Тип ресурса threatSubmission

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отправку угроз, которая является абстрактным типом для представления предполагаемой нежелательной почты, вредоносных программ, фишинга и заблокированных допустимых сообщений электронной почты; вредоносные программы, фишинговые и заблокированные допустимые URL-адреса; фишинг, вредоносные программы и заблокированные вложения в Microsoft Defender для Office 365 и подозрительные файлы для Microsoft Defender для конечной точки.

Этот ресурс также можно использовать для отправки ложных срабатываний, которые не должны быть заблокированы Microsoft Defender для Office 365; например, не нежелательной почты, безопасных URL-адресов и безопасных вложений электронной почты.

Это абстрактный тип. Наследует [от сущности](../resources/entity.md). Базовый тип [emailThreatSubmission](../resources/security-emailthreatsubmission.md), [urlThreatSubmission](../resources/security-urlthreatsubmission.md), [fileThreatSubmissin](../resources/security-filethreatsubmission.md).

## <a name="properties"></a>Свойства
| Свойство        | Тип                       | Описание                                                                      |
|:----------------|:---------------------------|:---------------------------------------------------------------------------------|
| adminReview     | [security.submissionAdminReview](../resources/security-submissionadminreview.md)| Указывает свойство проверки администратора, которое состоит из того, кто просматривал отправку пользователя, когда и как она была определена. |
| category        | submissionCategory         | Указывает категорию отправки. Поддерживает `$filter = category eq 'value'`. Возможные значения: `notJunk`, `spam`, и `phishing``malware` `unkownFutureValue`.|
| clientSource    | submissionClientSource     | Указывает источник отправки. Возможные значения: `microsoft`и  `other` `unkownFutureValue`. |
| contentType     | submissionContentType      | Указывает тип отправляемого содержимого. Возможные значения: `email`, `url`, и `file``app` `unkownFutureValue`.  |
| createdBy       | [security.submissionUserIdentity](../resources/security-submissionuseridentity.md)     | Указывает, кто отправил сообщение электронной почты как угрозу. Поддерживает `$filter = createdBy/email eq 'value'`. |
| createdDateTime | DateTimeOffset  | Указывает, когда была создана отправка угрозы. Поддерживает `$filter = createdDateTime ge 2022-01-01T00:00:00Z and createdDateTime lt 2022-01-02T00:00:00Z`.             |
| id              | String                     | Указывает идентификатор отправки угрозы. |
| result          | [security.submissionResult](../resources/security-submissionresult.md)          | Указывает результат анализа, выполненного корпорацией Майкрософт.  |
| source          | submissionSource           | Указывает роль отправителя. Поддерживает `$filter = source eq 'value'`. Возможные значения: `administrator`и  `user` `unkownFutureValue`.  |
| status          | longRunningOperationStatus | Указывает, была ли отправка угроз проанализирована корпорацией Майкрософт. Поддерживает `$filter = status eq 'value'`. Возможные значения: , , , , и `failed``skipped` `unkownFutureValue`. `succeeded``running``notStarted` |
| tenantId        | String                     | Указывает идентификатор клиента отправителя. Не требуется при создании с помощью `POST` операции. Он извлекается из маркера после вызова API. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.threatSubmission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.threatSubmission",
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
  "clientSource": "String"
}
```

