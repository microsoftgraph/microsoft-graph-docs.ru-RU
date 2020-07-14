---
title: Тип ресурса Виндовсупдатестате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25b15487be765de8c45896b10101671359e2659e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122485"
---
# <a name="windowsupdatestate-resource-type"></a>Тип ресурса Виндовсупдатестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсупдатестатес](../api/intune-shared-windowsupdatestate-list.md)|Коллекция [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md)|Список свойств и связей объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .|
|[Получение Виндовсупдатестате](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Чтение свойств и связей объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .|
|[Создание Виндовсупдатестате](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Создание нового объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .|
|[Удаление Виндовсупдатестате](../api/intune-shared-windowsupdatestate-delete.md)|Отсутствует|Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).|
|[Обновление Виндовсупдатестате](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Обновление свойств объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Это идентификатор объекта.|
|deviceId|String|Идентификатор устройства.|
|userId|String|Идентификатор пользователя.|
|deviceDisplayName|String|Отображаемое имя устройства.|
|userPrincipalName|Строка|Имя участника пользователя.|
|status|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Состояние Windows удпате. Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|куалитюпдатеверсион|String|Версия устройства для обновления качества.|
|феатуреупдатеверсион|String|Текущая версия обновления компонентов устройства.|
|ластскандатетиме|DateTimeOffset|Дата и время, когда агент обновления Windows успешно выполнил сканирование.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации устройства с Microsoft Intune.|

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



