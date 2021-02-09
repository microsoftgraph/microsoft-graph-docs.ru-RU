---
title: Тип ресурса windowsQualityUpdateProfile
description: Профиль обновления качества Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e540ed43dec833f8d55c72cef5db7780b921f32
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162453"
---
# <a name="windowsqualityupdateprofile-resource-type"></a>Тип ресурса windowsQualityUpdateProfile

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль обновления качества Windows

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateProfiles](../api/intune-softwareupdate-windowsqualityupdateprofile-list.md)|[Коллекция windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Список свойств и связей объектов [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Get windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-get.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Чтение свойств и связей объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Создание windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-create.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Создание объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Удаление windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-delete.md)|Нет|Удаляет [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Обновление windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-update.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Обновление свойств объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Действие assign](../api/intune-softwareupdate-windowsqualityupdateprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД политики Intune.|
|displayName|String|Отображаемая имя профиля.|
|description|String|Описание профиля, указанного пользователем.|
|expeditedUpdateSettings|[expeditedWindowsQualityUpdateSettings](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|Параметры ускорения обновления.|
|createdDateTime|DateTimeOffset|Дата создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого объекта обновления качества.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[Коллекция windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Список назначений группы профиля.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "String",
    "daysUntilForcedReboot": 1024
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




