---
title: Тип ресурса crossTenantAccessPolicyConfigurationPartner
description: Конфигурация для конкретного партнера, которая определяется для параметров входящего и исходящего трафика Azure AD B2B и прямого подключения B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86c9cb0d5009d8406c99fd38520dddb18936c2c8
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604747"
---
# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>Тип ресурса crossTenantAccessPolicyConfigurationPartner

Пространство имен: microsoft.graph

Конфигурация для конкретного партнера, которая определяется для параметров входящего и исходящего трафика Azure AD B2B и B2B direct connect.

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
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, которые имеют доступ к ресурсам через Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров, чтобы пользователи в вашей организации могли получать исходящий доступ к ресурсам в другой организации с помощью Azure AD B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, которые имеют доступ к ресурсам через прямое подключение Azure B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров, чтобы пользователи в вашей организации могли получать исходящий доступ к ресурсам в другой организации через Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию для партнеров для доверия другим утверждениям условного доступа из внешних Azure AD организаций. |
| isServiceProvider | Boolean | Определяет, является ли конфигурация для конкретного партнера поставщиком облачных служб для вашей организации. |
| tenantId | String | Идентификатор клиента для партнерской Azure AD организации. Только для чтения. Ключ.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
