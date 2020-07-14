---
title: Тип ресурса Виндовсфеатуреупдатепрофиле
description: Профиль обновления компонентов Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a800a24cd4eb41258a060b67f77f0eed5e479817
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122527"
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
|[Удаление Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|Отсутствует|Удаляет объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).|
|[Обновление Виндовсфеатуреупдатепрофиле](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Обновление свойств объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .|
|[Действие assign](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта.|
|displayName|Строка|Отображаемое имя профиля.|
|description|String|Описание профиля, указанного пользователем.|
|феатуреупдатеверсион|String|Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля. Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.|
|createdDateTime|DateTimeOffset|Дата и время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения профиля.|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого элемента обновления компонента.|

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



