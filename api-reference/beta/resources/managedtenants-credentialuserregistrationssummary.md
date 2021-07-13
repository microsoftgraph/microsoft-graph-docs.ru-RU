---
title: тип ресурса credentialUserRegistrationsSummary
description: Представляет сводку Azure Active Directory регистраций пользователей учетных данных для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 43a3f5cd39e8c151c71f976042e9bb33ae527dc4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402538"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>тип ресурса credentialUserRegistrationsSummary

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку Azure Active Directory регистраций пользователей учетных данных для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) collection|Получите список объектов [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) и их свойств.|
|[Получите credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Ознакомьтесь с свойствами и отношениями объекта [credentialUserRegistrationsSummary.](../resources/managedtenants-credentialuserregistrationssummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|mfaAndSsprCapableUserCount|Int32|Количество пользователей, способных выполнять многофакторную проверку подлинности или сброс пароля самообслуживления. Необязательно. Только для чтения.|
|mfaConditionalAccessPolicyState|String|Состояние политики условного доступа, которая обеспечивает многофакторную проверку подлинности. Необязательно. Только для чтения.|
|mfaRegisteredUserCount|Int32|Количество пользователей, зарегистрированных для многофакторной проверки подлинности. Необязательно. Только для чтения.|
|securityDefaultsEnabled|Boolean|Флаг, указывающий, включен ли по умолчанию безопасность удостоверений. Необязательно. Только для чтения.|
|ssprEnabledUserCount|Int32|Число пользователей, включенных для сброса пароля самообслуживки. Необязательно. Только для чтения.|
|ssprRegisteredUserCount|Int32|Число пользователей, зарегистрированных для сброса пароля самообслуживки. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|
|totalUserCount|Int32|Общее число пользователей в этом управляемом клиенте. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
