---
title: Тип ресурса Девицеманажементресаурцеакцесспрофилеассигнмент
description: Сущность, описывающая параметры уровня клиента для производных учетных данных
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d52845a705cce3ef7a2171b151c014c994cd78a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302303"
---
# <a name="devicemanagementresourceaccessprofileassignment-resource-type"></a>Тип ресурса Девицеманажементресаурцеакцесспрофилеассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая параметры уровня клиента для производных учетных данных

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементресаурцеакцесспрофилеассигнментс](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-list.md)|Коллекция [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список свойств и связей объектов [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Получение Девицеманажементресаурцеакцесспрофилеассигнмент](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-get.md)|[девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Чтение свойств и связей объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Создание Девицеманажементресаурцеакцесспрофилеассигнмент](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-create.md)|[девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Создание нового объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|
|[Удаление Девицеманажементресаурцеакцесспрофилеассигнмент](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-delete.md)|Нет|Удаляет объект [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).|
|[Обновление Девицеманажементресаурцеакцесспрофилеассигнмент](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-update.md)|[девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Обновление свойств объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначений|
|intent|[девицеманажементресаурцеакцесспрофилеинтент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|Цель назначения для профиля доступа к ресурсам. Возможные значения: `apply`, `remove`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для профиля доступа к ресурсу.|
|Идентификатор|String|Идентификатор источника назначения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "sourceId": "String"
}
```




