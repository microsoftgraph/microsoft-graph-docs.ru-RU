---
title: Тип ресурса crossTenantAccessPolicyConfigurationPartner
description: Конфигурация для конкретного партнера, которая определяется для параметров входящего и исходящего трафика службы совместной работы Azure AD B2B и прямого подключения B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 73849d18cce7639e82e5b56a37f46ce7705b707f
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103039"
---
# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>Тип ресурса crossTenantAccessPolicyConfigurationPartner

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конфигурация для конкретного партнера, которая определяется для параметров входящего и исходящего трафика azure AD B2B и службы прямого подключения B2B.

Для любого свойства, определяемого партнером `null`, эти параметры наследуют поведение, настроенное в параметрах межтенантного доступа по [умолчанию](../resources/crosstenantaccesspolicyconfigurationdefault.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление партнеров](../api/crosstenantaccesspolicy-list-partners.md) | [Коллекция crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Получение списка всех конфигураций для партнеров. |
| [Создание crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Создайте конфигурацию для конкретного партнера. |
| [Получение crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Чтение параметров конфигурации для конкретного партнера. |
| [Обновление crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Обновите свойства конфигурации для конкретного партнера. |
| [Удаление crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | Нет | Удалите конфигурацию для конкретного партнера. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, которые имеют доступ к ресурсам через службу совместной работы Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров, чтобы пользователи в вашей организации могли получать исходящий доступ к ресурсам в другой организации с помощью службы совместной работы Azure AD B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, которые имеют доступ к ресурсам через прямое подключение Azure B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для конкретного партнера для пользователей в вашей организации, которые будут получать исходящий доступ к ресурсам в другой организации через прямое подключение Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию для партнеров, чтобы доверять другим утверждениям условного доступа от внешних организаций Azure AD. |
| isServiceProvider | Логическое | Определяет, является ли конфигурация для конкретного партнера поставщиком облачных служб для вашей организации. |
| tenantId | String | Идентификатор клиента для партнерской организации Azure AD. Только для чтения. Ключ.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "tenantId",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "tenantId": "String (identifier)",
  "inboundTrust": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
  },
  "b2bCollaborationOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bCollaborationInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "isServiceProvider": "Boolean"
}
```
