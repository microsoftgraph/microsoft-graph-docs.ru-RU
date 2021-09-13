---
title: тип ресурса groupPolicyConfigurationAssignment
description: Объект назначения конфигурации групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20f3401a78209ddb55fd363ada3d79f0cc986371
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017354"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>тип ресурса groupPolicyConfigurationAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект назначения конфигурации групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyConfigurationAssignments](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|[коллекция groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Список свойств и связей объектов [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Get groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Чтение свойств и связей объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Создание groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Создайте новый [объект GroupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|
|[Удаление groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|Нет|Удаляет [группуPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).|
|[Update groupPolicyConfigurationAssignment](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Обновление свойств объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп был ориентирован на конфигурацию групповой политики.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



