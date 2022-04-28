---
title: Тип ресурса crossTenantAccessPolicyConfigurationDefault
description: Конфигурация по умолчанию, определенная для параметров входящего и исходящего трафика службы совместной работы Azure AD B2B и прямого подключения B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb4df32d047a695952a3ac0b91bb3188f90c190
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103023"
---
# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>Тип ресурса crossTenantAccessPolicyConfigurationDefault

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конфигурация по умолчанию, определенная для параметров входящего и исходящего трафика службы совместной работы Azure AD B2B и прямого подключения B2B.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Получите конфигурацию по умолчанию для совместной работы B2B и параметров прямого подключения B2B для входящего и исходящего трафика.|
|[Обновление crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|Нет|Обновите конфигурацию по умолчанию для совместной работы B2B и параметров прямого подключения B2B для входящего и исходящего трафика.|
|[Сброс до системного значения по умолчанию](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|Нет|Сбросьте конфигурацию по умолчанию для политики межтенантного доступа к параметрам системы по умолчанию.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей из других организаций, которые имеют доступ к ресурсам через службу совместной работы Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей в организации, которые будут получать исходящий доступ к ресурсам в другой организации с помощью службы совместной работы Azure AD B2B. |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей из других организаций, которые имеют доступ к ресурсам через прямое подключение Azure AD B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей в вашей организации, которые будут получать исходящий трафик для доступа к ресурсам в другой организации через прямое подключение Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию по умолчанию для доверия другим утверждениям условного доступа от внешних организаций Azure AD. |
| isServiceDefault | Логическое | Если `true`используется конфигурация по умолчанию, задана конфигурация системы по умолчанию. Если `false`параметры по умолчанию настроены. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
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
  "isServiceDefault": "Boolean"
}
```
