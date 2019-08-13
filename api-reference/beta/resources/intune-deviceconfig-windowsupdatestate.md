---
title: Тип ресурса Виндовсупдатестате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47f2e2668634fed4d24d952d08b2b4a90f33c332
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337680"
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
|куалитюпдатеверсион|String|Версия устройства для обновления качества.|
|феатуреупдатеверсион|String|Текущая версия обновления компонентов устройства.|
|ластскандатетиме|DateTimeOffset|Дата и время, когда агент обновления Windows успешно выполнил сканирование.|
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



