---
title: тип ресурса windowsQualityUpdateProfile
description: Windows Профиль обновления качества
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44fcad282f98e54bae569bf78b4c7464f430d915
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029803"
---
# <a name="windowsqualityupdateprofile-resource-type"></a>тип ресурса windowsQualityUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Профиль обновления качества

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateProfiles](../api/intune-softwareupdate-windowsqualityupdateprofile-list.md)|[коллекция windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Список свойств и связей [объектов WindowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Get windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-get.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Чтение свойств и связей [объекта WindowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Создание windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-create.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Создайте [новый объект WindowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Удаление windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-delete.md)|Нет|Удаляет [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).|
|[Обновление windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-update.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|Обновление свойств объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|
|[Действие assign](../api/intune-softwareupdate-windowsqualityupdateprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID политики Intune.|
|displayName|String|Имя отображения для профиля.|
|description|String|Описание профиля, указанного пользователем.|
|expeditedUpdateSettings|[expeditedWindowsQualityUpdateSettings](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|Параметры ускоренного обновления.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого объекта обновления качества.|
|releaseDateDisplayName|String|Содружественная дата выпуска для отображения для выпуска обновления качества|
|deployableContentDisplayName|String|Удобное отображаемое имя развернутого контента профиля обновления качества|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Список групповых назначений профиля.|

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
  ],
  "releaseDateDisplayName": "String",
  "deployableContentDisplayName": "String"
}
```



