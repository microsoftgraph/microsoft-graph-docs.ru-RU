---
title: Тип ресурса Девицеманажементресаурцеакцесспрофилебасе
description: Тип базового профиля для доступа к ресурсам
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df8389670d636d5ab556339ae4fc89217043663e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337133"
---
# <a name="devicemanagementresourceaccessprofilebase-resource-type"></a>Тип ресурса Девицеманажементресаурцеакцесспрофилебасе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип базового профиля для доступа к ресурсам

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементресаурцеакцесспрофилебасес](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|Коллекция [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Список свойств и связей объектов [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) .|
|[Получение Девицеманажементресаурцеакцесспрофилебасе](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Чтение свойств и связей объекта [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) .|
|[Действие assign](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|Коллекция [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор профиля|
|version|Int32|Версия профиля|
|displayName|String|Отображаемое имя профиля|
|description|String|Описание профиля|
|креатиондатетиме|DateTimeOffset|Создан профиль DateTime|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение профиля DateTime|
|roleScopeTagIds|Коллекция строк|Теги областей|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список назначений для профиля конфигурации устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




