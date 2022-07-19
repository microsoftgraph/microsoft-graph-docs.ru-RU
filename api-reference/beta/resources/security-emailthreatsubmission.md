---
title: Тип ресурса emailThreatSubmission
description: Сообщает о подозрительной нежелательной почте, вредоносных программах или фишинговых сообщениях Microsoft Defender для Office 365.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 387d4531a6f2e4d4b9184e4006ae43ddac4c15ed
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856854"
---
# <a name="emailthreatsubmission-resource-type"></a>Тип ресурса emailThreatSubmission

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип для сообщения о подозрительной спаме, вредоносных программах или фишинговых сообщениях электронной почты Microsoft Defender для Office 365. Вы также можете отправлять ложные срабатывания, которые не должны были быть заблокированы Microsoft Defender для Office 365 например, сообщения электронной почты неправильно классифицируются как нежелательные или нежелательные.

Наследуется [от threatSubmission](../resources/security-threatsubmission.md). Базовый тип [emailContentThreatSubmission](../resources/security-emailcontentthreatsubmission.md) и [emailUrlThreatSubmission](../resources/security-emailurlthreatsubmission.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов emailThreatSubmission](../api/security-emailthreatsubmission-list.md)|[Коллекция microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Получение списка объектов [emailThreatSubmission](../resources/security-emailthreatsubmission.md) и их свойств.|
|[Создание emailThreatSubmission](../api/security-emailthreatsubmission-post-emailthreats.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Создайте объект [emailThreatSubmission](../resources/security-emailthreatsubmission.md) .|
|[Получение emailThreatSubmission](../api/security-emailthreatsubmission-get.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Чтение свойств и связей объекта [emailThreatSubmission](../resources/security-emailthreatsubmission.md) .|
|[Отзыв](../api/security-emailthreatsubmission-review.md)|Нет|Просмотрите отправку угроз от конечного пользователя администратором.|

## <a name="properties"></a>Свойства
| Свойство     | Тип    | Описание    |
|:-----------------------------|:-----------------------------|:-------------------------------------------------------------------------------------------------------|
| attackSimulationInfo         | [security.attackSimulationInfo](../resources/security-attacksimulationinfo.md) | Если сообщение электронной почты является имитацией фишинга, это поле не будет иметь значение NULL.|
| internetMessageId            | String                       | Указывает идентификатор отправляемого сообщения электронной почты в Интернете. Эти сведения присутствуют в заголовке электронной почты. |
| originalCategory             | submissionCategory           | Исходная категория отправки. Возможные значения: `notJunk`, `spam`, и `phishing``malware` `unkownFutureValue`. |
| receivedDateTime             | DateTimeOffset               | Указывает метку даты и времени, когда было получено сообщение электронной почты.  | 
| recipientEmailAddress        | Строка                       | Указывает адрес электронной почты (в формате smtp) получателя, который получил сообщение электронной почты. |
| sender                       | String                       | Указывает адрес электронной почты отправителя. | 
| senderIP                     | String                       | Указывает IP-адрес отправителя. |
| subject                      | String                       | Указывает тему сообщения электронной почты. |
| tenantAllowOrBlockListAction | [security.tenantAllowOrBlockListAction](../resources/security-tenantalloworblocklistaction.md) | Он используется для автоматического добавления разрешений для таких компонентов, как URL-адрес, файл, отправитель; , которые считаются недопустимыми корпорацией Майкрософт, чтобы в будущем можно было разрешить аналогичные сообщения. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmission",
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
  "recipientEmailAddress": "String",
  "internetMessageId": "String",
  "subject": "String",
  "sender": "String",
  "senderIP": "String",
  "receivedDateTime": "String (timestamp)",
  "originalCategory": "String",
  "attackSimulationInfo": {
    "@odata.type": "microsoft.graph.security.attackSimulationInfo"
  },
  "tenantAllowOrBlockListAction": {
    "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
  }
}
```

