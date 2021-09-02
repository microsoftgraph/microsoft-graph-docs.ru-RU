---
title: тип ресурса deviceManagementResourceAccessProfileBase
description: Тип базового профиля для доступа к ресурсам
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e6a182af3aff9851095d689ebc41923534a143e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806581"
---
# <a name="devicemanagementresourceaccessprofilebase-resource-type"></a>тип ресурса deviceManagementResourceAccessProfileBase

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип базового профиля для доступа к ресурсам

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementResourceAccessProfileBases](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|[коллекция deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Список свойств и связей [объектов deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[Get deviceManagementResourceAccessProfileBase](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Чтение свойств и связей [объекта deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[Действие assign](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|[коллекция deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Пока не задокументировано.|
|[действие queryByPlatformType](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-querybyplatformtype.md)|[коллекция deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Н/Д|

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

## <a name="relationships"></a>Связи
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



