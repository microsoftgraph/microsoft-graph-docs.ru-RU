---
title: тип ресурса windowsFeatureUpdateProfile
description: Windows Профиль обновления функций
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8de71467651f732732b3eaaa3dfd88a79eaaf121
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029873"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a>тип ресурса windowsFeatureUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Профиль обновления функций

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsFeatureUpdateProfiles](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|[коллекция windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Список свойств и связей [объектов windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Get windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Чтение свойств и связей [объекта windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Создание windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Создайте [новый объект windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Удаление windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|Нет|Удаляет [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).|
|[Обновление windowsFeatureUpdateProfile](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Обновление свойств объекта [windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|
|[Действие assign](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта.|
|displayName|String|Имя отображения профиля.|
|description|String|Описание профиля, указанного пользователем.|
|featureUpdateVersion|String|Версия обновления функций, которая будет развернута на устройствах, на которые ориентирован этот профиль. Версия может быть любой поддерживаемой версией, например 1709, 1803 или 1809 и так далее.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого объекта обновления функций.|
|deployableContentDisplayName|String|Удобное отображаемое имя развернутого контента профиля обновления качества|
|endOfSupportDate|DateTimeOffset|Последняя поддерживаемая дата обновления функций|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Список групповых назначений профиля.|

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
  ],
  "deployableContentDisplayName": "String",
  "endOfSupportDate": "String (timestamp)"
}
```



