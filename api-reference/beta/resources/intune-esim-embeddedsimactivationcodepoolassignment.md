---
title: тип ресурса embeddedSIMActivationCodePoolAssignment
description: Встраиваемый объект назначения пула кодов активации SIM-кода назначает определенную встроенную группу устройств AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29617a21c858ec9ef5f5ee619d8f46f9746fdf3bd0a55c0dbf82761f8ff98db0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244647"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>тип ресурса embeddedSIMActivationCodePoolAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встраиваемый объект назначения пула кодов активации SIM-кода назначает определенную встроенную группу устройств AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список встроенныхSIMActivationCodePoolAssignments](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|[коллекция embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Список свойств и связей встроенных [объектовSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Get embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Чтение свойств и связей встроенного [объектаSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Создание встроенногоSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Создание нового [объекта embeddedSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|
|[Удаление встроенногоSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Нет|Удаляет [встроенныйSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[Обновление встроенныхSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Обновление свойств встроенного [объектаSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для встроенного пула активации SIM-кода. Созданное в системе значение, назначенное при его создания.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп, целевых для встроенного пула кодов активации SIM.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




