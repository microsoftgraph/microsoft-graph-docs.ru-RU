---
title: Тип ресурса Виндовсфеатуреупдатепрофиле
description: Профиль обновления компонентов Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2157fccff9cbd6a1618b5989b91bb95edae576c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702238"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a>Тип ресурса Виндовсфеатуреупдатепрофиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль обновления компонентов Windows

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсфеатуреупдатепрофилес](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|Коллекция [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Список свойств и связей объектов [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .|
|[Получение Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Чтение свойств и связей объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .|
|[Создание Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Создание нового объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .|
|[Удаление Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|Нет|Удаляет объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).|
|[Обновление Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Обновление свойств объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .|
|[Действие assign](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор объекта.|
|displayName|Строка|Отображаемое имя профиля.|
|description|Строка|Описание профиля, указанного пользователем.|
|феатуреупдатеверсион|Строка|Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля. Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.|
|createdDateTime|DateTimeOffset|Дата и время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения профиля.|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого элемента обновления компонента.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Список назначений групп для профиля.|
|девицеупдатестатес|Коллекция [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md)|Список состояний устройств, для которых предназначен данный профиль|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "featureUpdateVersion": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```





