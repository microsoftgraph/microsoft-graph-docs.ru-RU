---
title: тип ресурса cloudPcAuditActor
description: Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5cd851d22d20eb5d0e466cae7b799ad70bd390a2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766315"
---
# <a name="cloudpcauditactor-resource-type"></a>тип ресурса cloudPcAuditActor

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.

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
|remoteUserId|Строка|Делегированная ид пользователя-партнера.|

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
