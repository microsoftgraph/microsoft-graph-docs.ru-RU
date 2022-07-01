---
title: Тип ресурса crossTenantAccessPolicyConfigurationDefault
description: Конфигурация по умолчанию, определенная для параметров входящего и исходящего трафика Azure AD B2B и прямого подключения B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 08d32f51db26721205806b4b730ae6f77c0b4b98
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604750"
---
# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>Тип ресурса crossTenantAccessPolicyConfigurationDefault

Пространство имен: microsoft.graph

Конфигурация по умолчанию, определенная для параметров входящего и исходящего трафика Azure AD B2B и прямого подключения B2B.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Получите конфигурацию по умолчанию для совместной работы B2B и параметров прямого подключения B2B для входящего и исходящего трафика.|
|[Обновление crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|Нет|Обновите конфигурацию по умолчанию для совместной работы B2B и параметров прямого подключения B2B для входящего и исходящего трафика.|
|[Сброс до системного значения по умолчанию](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|Нет|Сбросьте конфигурацию по умолчанию для политики межтенантного доступа к параметрам системы по умолчанию.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей из других организаций, которые имеют доступ к ресурсам Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей в организации, которые будут получать исходящий доступ к ресурсам в другой организации с помощью Azure AD B2B. |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей из других организаций, которые имеют доступ к ресурсам через Azure AD B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для исходящих пользователей в организации для доступа к ресурсам в другой организации через Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию по умолчанию для доверия другим утверждениям условного доступа от внешних Azure AD организаций. |
| isServiceDefault | Boolean | Если `true`используется конфигурация по умолчанию, задана конфигурация системы по умолчанию. Если `false`параметры по умолчанию настроены. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
