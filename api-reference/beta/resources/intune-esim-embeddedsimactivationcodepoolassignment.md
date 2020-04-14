---
title: Тип ресурса Ембеддедсимактиватионкодепулассигнмент
description: Внедренный объект назначения пула кода активации SIM-карты назначает определенный Ембеддедсимактиватионкодепул группе устройств AAD.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96863bafc774389e7d287bc7af9b8b2073b31c72
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442807"
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



