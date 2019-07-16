---
title: Тип ресурса Виндовсупдатестате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a023e4f74fe7a0abc96a47b79c7da7104617c9d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726139"
---
# <a name="windowsupdatestate-resource-type"></a>Тип ресурса Виндовсупдатестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсупдатестатес](../api/intune-deviceconfig-windowsupdatestate-list.md)|Коллекция [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md)|Список свойств и связей объектов [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Получение Виндовсупдатестате](../api/intune-deviceconfig-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Чтение свойств и связей объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Создание Виндовсупдатестате](../api/intune-deviceconfig-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Создание нового объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .|
|[Удаление Виндовсупдатестате](../api/intune-deviceconfig-windowsupdatestate-delete.md)|Нет|Удаляет объект [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md).|
|[Обновление Виндовсупдатестате](../api/intune-deviceconfig-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|Обновление свойств объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Это идентификатор объекта.|
|deviceId|String|Идентификатор устройства.|
|userId|String|Идентификатор пользователя.|
|deviceDisplayName|String|Отображаемое имя устройства.|
|userPrincipalName|Строка|Имя участника пользователя.|
|status|[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)|Состояние Windows удпате. Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|Куалитюпдатеверсион|String|Версия устройства для обновления качества.|
|Феатуреупдатеверсион|String|Текущая версия обновления компонентов устройства.|
|Ластскандатетиме|DateTimeOffset|Дата и время, когда агент обновления Windows успешно выполнил сканирование.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации устройства с Microsoft Intune.|

## <a name="relationships"></a>Отношения
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





