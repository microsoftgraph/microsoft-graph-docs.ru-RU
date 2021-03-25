---
title: тип ресурса deviceManagementResourceAccessProfileBase
description: Тип базового профиля для доступа к ресурсам
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d795d99e2d3808268100c22ac8d9840edd96c85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151818"
---
# <a name="devicemanagementresourceaccessprofilebase-resource-type"></a>тип ресурса deviceManagementResourceAccessProfileBase

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип базового профиля для доступа к ресурсам

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementResourceAccessProfileBases](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|[коллекция deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Список свойств и связей [объектов deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[Get deviceManagementResourceAccessProfileBase](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Чтение свойств и связей [объекта deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[Действие assign](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|[коллекция deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Пока не задокументировано.|
|[действие queryByPlatformType](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-querybyplatformtype.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор профиля|
|version|Int32|Версия профиля|
|displayName|Строка|Имя отображения профиля|
|description|Строка|Описание профиля|
|creationDateTime|DateTimeOffset|Создан профиль DateTime|
|lastModifiedDateTime|DateTimeOffset|Последний изменен профиль DateTime|
|roleScopeTagIds|Коллекция String|Теги области|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список назначений для профиля конфигурации устройства.|

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




