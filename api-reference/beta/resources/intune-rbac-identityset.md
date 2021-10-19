---
title: Тип ресурса identitySet
description: Набор удостоверений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 427c627ac25e7ed795f6891c3deac470471b2ee8
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60481610"
---
# <a name="identityset-resource-type"></a>Тип ресурса identitySet

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Набор удостоверений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|application|[identity](../resources/intune-rbac-identity.md)|Удостоверение приложения. Это свойство доступно только для чтения.|
|device;|[identity](../resources/intune-rbac-identity.md)|Удостоверение устройства. Это свойство доступно только для чтения.|
|пользователь|[identity](../resources/intune-rbac-identity.md)|Удостоверение пользователя. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identitySet",
  "application": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "user": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  }
}
```



