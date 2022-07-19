---
title: Тип ресурса emailThreatSubmissionPolicy
description: Представляет рекомендации организации по созданию отчетов о потенциальных угрозах и спаме.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d34e239e9c7717aaf21d2619a47ab3a005b42d7b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856915"
---
# <a name="emailthreatsubmissionpolicy-resource-type"></a>Тип ресурса emailThreatSubmissionPolicy

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет рекомендации организации по отправке сообщений о потенциальных угрозах и спаме. Он используется для настройки интерфейса отправки угроз конечным пользователям вашей организации при отправке сообщений о потенциальных угрозах и спаме в Microsoft Outlook.


Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление emailThreatSubmissionPolicies](../api/security-emailthreatsubmissionpolicy-list.md)|[Коллекция microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Получение списка объектов [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) и их свойств.|
|[Создание emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-post-emailthreatsubmissionpolicies.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Создайте объект [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Получение emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-get.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Чтение свойств и связей объекта [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Обновление emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-update.md)|Нет|Обновление свойств объекта [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Удаление emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-delete.md)|Нет|Удаляет объект [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|

## <a name="properties"></a>Свойства
| Свойство                                 | Тип    | Описание                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | Строка  | Указывает адрес электронной почты отправителя, с которого будут отправляться уведомления по электронной почте конечным пользователям, чтобы сообщить им, является ли сообщение спамом, фишингом или очисткой. Значение по умолчанию — `null`. Необязательный для создания.                   |
| customizedReportRecipientEmailAddress    | String  | Указывает место назначения, куда будут отправляться сообщения от конечных пользователей, когда они сообщают что-то как фишинговое, нежелательное или не нежелательное. Значение по умолчанию — `null`. Необязательный для создания. |
| id                                       | String  | Поддерживается только один идентификатор. Значение по умолчанию — `DefaultReportSubmissionPolicy`. |
| isAlwaysReportEnabledForUsers            | Логический | Указывает, могут ли конечные пользователи сообщать о сообщении как спаме, фишинге или нежелательной почте напрямую без подтверждения (всплывающего окна). Значение по умолчанию — `true`.  Необязательный для создания.          |
| isAskMeEnabledForUsers                   | Логический | Указывает, могут ли пользователи подтвердить использование всплывающего окна перед отправкой сообщений как спама, фишинга или нежелательной почты. Значение по умолчанию — `true`.  Необязательный для создания.   |
| isCustomizedMessageEnabled               | Логический | Указывает, настроены ли уведомления по электронной почте, отправляемые конечным пользователям для уведомления о фишинге, спаме или нежелательной почте. Значение по умолчанию — `false`. Необязательный для создания.    |
| isCustomizedMessageEnabledForPhishing    | Логический | Если этот параметр включен, настроенное сообщение отображается только в том случае, если сообщение электронной почты отображается как фишинговое. Значение по умолчанию — `false`. Необязательный для создания. |
| isCustomizedNotificationSenderEnabled    | Логический | Указывает, следует ли использовать набор адресов электронной почты отправителя с помощью customizedNotificationSenderEmailAddress для отправки уведомлений по электронной почте конечным пользователям. Значение по умолчанию — `false`. Необязательный для создания.  |
| isNeverReportEnabledForUsers             | Логический | Указывает, могут ли пользователи просто переместить сообщение из одной папки в другую на основе действий спама, фишинга или нежелательной почты без фактического сообщения о нем. Значение по умолчанию — `true`. Необязательный для создания.         |
| isOrganizationBrandingEnabled            | Логический | Указывает, следует ли использовать логотип фирменной символики в уведомлениях по электронной почте, отправляемых конечным пользователям. Значение по умолчанию — `false`. Необязательный для создания.        |
| isReportFromQuarantineEnabled            | Логический | Указывает, могут ли пользователи отправлять данные со страницы карантина. Значение по умолчанию — `true`. Необязательный для создания.  |
| isReportToCustomizedEmailAddressEnabled  | Логический | Указывает, следует ли отправлять сообщения электронной почты, сообщаемые конечными пользователями, в пользовательский почтовый ящик, настроенный с помощью customizedReportRecipientEmailAddress.  Значение по умолчанию — `false`. Необязательный для создания.              |
| isReportToMicrosoftEnabled               | Логический | Если этот параметр включен, сообщение электронной почты будет отправлено в корпорацию Майкрософт для анализа. Значение по умолчанию — `false`. Требуется для создания.  |
| isReviewEmailNotificationEnabled         | Логический | Указывает, отправляется ли уведомление по электронной почте пользователю, который сообщил сообщение электронной почты при проверке администратором. Значение по умолчанию — `false`.. Необязательный для создания.  |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmissionPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
  "id": "String (identifier)",
  "isReportToMicrosoftEnabled": "Boolean",
  "isReportToCustomizedEmailAddressEnabled": "Boolean",
  "isAskMeEnabledForUsers": "Boolean",
  "isAlwaysReportEnabledForUsers": "Boolean",
  "isNeverReportEnabledForUsers": "Boolean",
  "isCustomizedMessageEnabledForPhishing": "Boolean",
  "isCustomizedMessageEnabled": "Boolean",
  "customizedReportRecipientEmailAddress": "String",
  "isReviewEmailNotificationEnabled": "Boolean",
  "isCustomizedNotificationSenderEnabled": "Boolean",
  "isOrganizationBrandingEnabled": "Boolean",
  "customizedNotificationSenderEmailAddress": "String",
  "isReportFromQuarantineEnabled": "Boolean"
}
```

