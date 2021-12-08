---
title: тип ресурса deviceAndAppManagementAssignedRoleDetails
description: Набор определений ролей и назначений ролей, присвоенных пользователю.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9369faebceaabd27da230e4888914fee9c5e6133
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342421"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>тип ресурса deviceAndAppManagementAssignedRoleDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Набор определений ролей и назначений ролей, присвоенных пользователю.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|roleDefinitionIds|Коллекция String|Определения ролей для specifc Role Definitions, назначенного пользователю. Это свойство доступно только для чтения.|
|roleAssignmentIds|Коллекция String|ID-данные назначения ролей для specifc Role Assignments, назначенного пользователю. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```




