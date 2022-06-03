---
title: Тип ресурса credentialUserRegistrationsSummary
description: Представляет сводку по регистрации пользователей учетных данных Azure Active Directory для данного управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 587925f16ab66cb6870102078ad2f885731c4832
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883861"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>Тип ресурса credentialUserRegistrationsSummary

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку по регистрации пользователей учетных данных Azure Active Directory для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[Коллекция microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Получение списка объектов [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) и их свойств.|
|[Получение credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Чтение свойств и связей объекта [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта. Обязательный аргумент. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления сущности на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|mfaAndSsprCapableUserCount|Int32|Количество пользователей, способных выполнять многофакторную проверку подлинности или самостоятельный сброс пароля. Необязательно. Только для чтения.|
|mfaConditionalAccessPolicyState|String|Состояние политики условного доступа, которая применяет многофакторную проверку подлинности. Необязательно. Только для чтения.|
|mfaExcludedUserCount|Int32|Количество пользователей в группе безопасности исключения многофакторной проверки подлинности (Microsoft 365 Lighthouse — исключения MFA). Необязательно. Только для чтения.|
|mfaRegisteredUserCount|Int32|Число пользователей, зарегистрированных для многофакторной проверки подлинности. Необязательно. Только для чтения.|
|securityDefaultsEnabled|Boolean|Флаг, указывающий, включены ли параметры безопасности удостоверений по умолчанию. Необязательно. Только для чтения.|
|ssprEnabledUserCount|Int32|Количество пользователей, которым разрешен самостоятельный сброс пароля. Необязательно. Только для чтения.|
|ssprRegisteredUserCount|Int32|Число пользователей, зарегистрированных для самостоятельного сброса пароля. Необязательно. Только для чтения.|
|tenantDisplayName|String|Отображаемое имя управляемого клиента. Обязательный аргумент. Только для чтения.|
|tenantId|String|Идентификатор клиента Azure Active Directory для [управляемого клиента](../resources/managedtenants-tenant.md). Обязательный аргумент. Только для чтения.|
|totalUserCount|Int32|Общее число пользователей в указанном управляемом клиенте. Необязательно. Только для чтения.|

## <a name="relationships"></a>Отношения
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
  "mfaExcludedUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
