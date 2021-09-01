---
title: тип ресурса windowsUpdateState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0f4e986483f5c4dce849295406ebad3cec721c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803751"
---
# <a name="windowsupdatestate-resource-type"></a>тип ресурса windowsUpdateState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|[коллекция windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Список свойств и связей [объектов WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Get windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Чтение свойств и связей [объекта WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Создание windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Создайте [новый объект WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|
|[Удаление windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|Нет|Удаляет [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).|
|[Обновление windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Обновление свойств объекта [WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Это Id объекта.|
|deviceId|String|ID устройства.|
|userId|String|ID пользователя.|
|deviceDisplayName|String|Имя отображения устройства.|
|userPrincipalName|String|Имя основного пользователя.|
|status|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Windows udpate. Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|Строка|Версия обновления качества устройства.|
|featureUpdateVersion|Строка|Текущая версия обновления функций устройства.|
|lastScanDateTime|DateTimeOffset|Время даты успешного Windows агента обновления.|
|lastSyncDateTime|DateTimeOffset|Последний раз, когда устройство синхронизируется с Microsoft Intune.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```



