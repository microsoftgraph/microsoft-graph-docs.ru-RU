---
title: тип ресурса cloudPcAuditActor
description: Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c0c63e9e9d0db7a5227f0ab7b818c8ab3d3944d9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211348"
---
# <a name="cloudpcauditactor-resource-type"></a>тип ресурса cloudPcAuditActor

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|type|[cloudPcAuditActorType](#cloudpcauditactortype-values)|Тип субъекта. Возможные значения включают `ItPro` `Application` , и `Partner` `Unknown` .|
|userPermissions|Коллекция строк|Список разрешений пользователей и разрешений приложений при выполнении события аудита.|
|applicationId|String|ID приложения Azure AD.|
|applicationDisplayName|String|Имя приложения.|
|userPrincipalName|String|Имя участника-пользователя (UPN).|
|servicePrincipalName|String|Имя субъекта-службы (SPN).|
|ipAddress|String|IP-адрес.|
|userId|String|ID пользователя Azure AD.|
|userRoleScopeTags|[коллекция cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md)|Список тегов области ролей.|
|remoteTenantId|String|Делегированная ид клиента-партнера.|
|remoteUserId|String|Делегированная ид пользователя-партнера.|

### <a name="cloudpcauditactortype-values"></a>значения cloudPcAuditActorType

|Member|Описание|
|:---|:---|
|itPro|Операция была выполнена ИТ-профессионалом.|
|приложение|Операция была выполнена приложением.|
|партнер|Операция была выполнена партнером.|
|unknown|Неизвестный актер.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
