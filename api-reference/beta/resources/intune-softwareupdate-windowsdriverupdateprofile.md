---
title: тип ресурса windowsDriverUpdateProfile
description: Windows профиля обновления драйвера
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee9304666ac2bc71485e25f8de16decc5c4d10fc
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712098"
---
# <a name="windowsdriverupdateprofile-resource-type"></a>тип ресурса windowsDriverUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows профиля обновления драйвера

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsDriverUpdateProfiles](../api/intune-softwareupdate-windowsdriverupdateprofile-list.md)|[коллекция windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Список свойств и связей [объектов WindowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Получить windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-get.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Чтение свойств и связей [объекта WindowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Создание windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-create.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Создайте [новый объект WindowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Удаление windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-delete.md)|Нет|Удаляет [windowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Обновление windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-update.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|Обновление свойств объекта [WindowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|
|[Действие assign](../api/intune-softwareupdate-windowsdriverupdateprofile-assign.md)|Нет|Н/Д|
|[Действие executeAction](../api/intune-softwareupdate-windowsdriverupdateprofile-executeaction.md)|[bulkDriverActionResult](../resources/intune-softwareupdate-bulkdriveractionresult.md)|Пока не задокументировано.|
|[syncInventory action](../api/intune-softwareupdate-windowsdriverupdateprofile-syncinventory.md)|Нет|Синхронизация инвентаризации драйверов WindowsDriverUpdateProfile.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID политики Intune.|
|displayName|String|Имя отображения для профиля.|
|description|String|Описание профиля, указанного пользователем.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Тип утверждения профиля обновления драйвера. Например, ручное или автоматическое утверждение. Возможные значения: `manual`, `automatic`.|
|deviceReporting|Int32|Количество устройств, сообщив об этом профиле|
|newUpdates|Int32|Количество новых обновлений драйвера, доступных для этого профиля.|
|deploymentDeferralInDays|Int32|Параметры отсрочки развертывания в днях, применимые только при автоматическом утверждении ApprovalType.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого объекта обновления драйвера.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md)|Список групповых назначений профиля.|
|driverInventories|[коллекция windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Запасы драйверов для этого профиля.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "approvalType": "String",
  "deviceReporting": 1024,
  "newUpdates": 1024,
  "deploymentDeferralInDays": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




