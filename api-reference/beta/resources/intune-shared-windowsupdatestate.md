---
title: Тип ресурса windowsUpdateState
description: Тип ресурса windowsUpdateState
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6cff1bf1becbd2e43967b05a210c7f3f5cfa864a
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900256"
---
# <a name="windowsupdatestate-resource-type"></a>Тип ресурса windowsUpdateState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|[Коллекция windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Список свойств и связей объектов [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Получение windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Чтение свойств и связей объекта [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Создание windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Создайте объект [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|
|[Удаление windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|Нет|Удаляет [объект windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).|
|[Обновление windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Обновление свойств объекта [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Это идентификатор сущности.|
|deviceId|String|Идентификатор устройства.|
|userId|String|Идентификатор пользователя.|
|deviceDisplayName|String|Отображаемое имя устройства.|
|userPrincipalName|String|Имя участника-пользователя.|
|status|[windowsUpdateStatus](/resources/intune-shared-windowsupdatestatus.md)|Состояние UDPATE Windows. Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|Строка|Версия обновления качества устройства.|
|featureUpdateVersion|Строка|Текущая версия обновления компонентов устройства.|
|lastScanDateTime|DateTimeOffset|Дата успешного сканирования агентом Центра обновления Windows.|
|lastSyncDateTime|DateTimeOffset|Дата последней синхронизации устройства с Microsoft Intune.|

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



