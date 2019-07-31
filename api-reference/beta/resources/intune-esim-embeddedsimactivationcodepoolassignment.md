---
title: Тип ресурса Ембеддедсимактиватионкодепулассигнмент
description: Внедренный объект назначения пула кода активации SIM-карты назначает определенный Ембеддедсимактиватионкодепул группе устройств AAD.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4115c2c6c64a621ec5264fa40d5a0f834e32ffb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998788"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>Тип ресурса Ембеддедсимактиватионкодепулассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Внедренный объект назначения пула кода активации SIM-карты назначает определенный Ембеддедсимактиватионкодепул группе устройств AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ембеддедсимактиватионкодепулассигнментс](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Список свойств и связей объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Получение Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[Ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Чтение свойств и связей объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Создание Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[Ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Создание нового объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|
|[Удаление Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Нет|Удаляет объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[Обновление Ембеддедсимактиватионкодепулассигнмент](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[Ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Обновление свойств объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначения внедренного пула кода активации SIM-карты. Созданное системой значение, назначаемое при создании.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп, на которые ссылается встроенный пул кода активации SIM-карты.|

## <a name="relationships"></a>Отношения
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





