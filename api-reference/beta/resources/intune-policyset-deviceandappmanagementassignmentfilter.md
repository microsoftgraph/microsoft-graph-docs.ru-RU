---
title: Тип ресурса Девицеандаппманажементассигнментфилтер
description: Класс, содержащий свойства, используемые для фильтра назначений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e3ea1fd9f7827fd8046de9024371022b61f56d6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793775"
---
# <a name="deviceandappmanagementassignmentfilter-resource-type"></a>Тип ресурса Девицеандаппманажементассигнментфилтер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для фильтра назначений.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеандаппманажементассигнментфилтерс](../api/intune-policyset-deviceandappmanagementassignmentfilter-list.md)|Коллекция [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Список свойств и связей объектов [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .|
|[Получение Девицеандаппманажементассигнментфилтер](../api/intune-policyset-deviceandappmanagementassignmentfilter-get.md)|[девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Чтение свойств и связей объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .|
|[Создание Девицеандаппманажементассигнментфилтер](../api/intune-policyset-deviceandappmanagementassignmentfilter-create.md)|[девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Создание нового объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .|
|[Удаление Девицеандаппманажементассигнментфилтер](../api/intune-policyset-deviceandappmanagementassignmentfilter-delete.md)|Нет|Удаляет объект [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).|
|[Обновление Девицеандаппманажементассигнментфилтер](../api/intune-policyset-deviceandappmanagementassignmentfilter-update.md)|[девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Обновление свойств объекта [девицеандаппманажементассигнментфилтер](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ фильтра назначений.|
|createdDateTime|DateTimeOffset|Время создания фильтра назначений.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения фильтра назначений.|
|displayName|Строка|DisplayName фильтра назначений.|
|description|String|Описание фильтра назначений.|
|platform|[девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Тип платформы устройств, к которым будет применяться фильтр назначений. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|правила|String|Определение правила для фильтра назначений.|
|roleScopeTags|Коллекция String|RoleScopeTags фильтра назначений.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ]
}
```



