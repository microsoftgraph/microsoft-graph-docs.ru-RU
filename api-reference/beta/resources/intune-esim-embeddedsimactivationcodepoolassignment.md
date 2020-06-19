---
title: Тип ресурса Ембеддедсимактиватионкодепулассигнмент
description: Внедренный объект назначения пула кода активации SIM-карты назначает определенный Ембеддедсимактиватионкодепул группе устройств AAD.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6205b80de2e58167cc5cb76194d84e5e7dece5c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793656"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>Тип ресурса Ембеддедсимактиватионкодепулассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Внедренный объект назначения пула кода активации SIM-карты назначает определенный Ембеддедсимактиватионкодепул группе устройств AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ембеддедсимактиватионкодепулассигнментс](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Список свойств и связей объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Получение Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Чтение свойств и связей объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Создание Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Создание нового объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Удаление Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Нет|Удаляет объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[Обновление Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Обновление свойств объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначения внедренного пула кода активации SIM-карты. Созданное системой значение, назначаемое при создании.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп, на которые ссылается встроенный пул кода активации SIM-карты.|

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



