---
title: тип ресурсов accessPackageSubject
description: В управлении правами Azure AD субъект назначения пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d8c8a7bb8943f88657392f06ea78ec2ec502d436
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651444"
---
# <a name="accesspackagesubject-resource-type"></a>тип ресурсов accessPackageSubject

Пространство имен: microsoft.graph


В управлении правами [Azure AD](entitlementmanagement-overview.md)субъект пакета доступа — это пользователь, руководитель службы или другая сущность, которую можно настроить для запроса или присвоения пакета доступа.  Он может представлять запросителя из связанной организации, который еще не находится в клиенте.

## <a name="methods"></a>Методы

Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени субъекта.|
|email|String|Адрес электронной почты субъекта.|
|id|String|Только для чтения.|
|objectId|String|Идентификатор объекта субъекта. `null` если субъект еще не является пользователем в клиенте.|
|onPremisesSecurityIdentifier|String|Строковая представление идентификатора безопасности субъекта, если оно известно, или если субъект не имеет `null` идентификатора безопасности.|
|principalName|String|Основное имя, если известно, субъекта.|
|subjectType|accessPackageSubjectType|Тип ресурса субъекта. Допустимые значения: `notSpecified`, `user`, `servicePrincipal`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|connectedOrganization|[connectedOrganization](connectedorganization.md)|Подключенная организация субъекта. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "objectId": "String",
  "onPremisesSecurityIdentifier": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "subjectType": "String"
}
```

