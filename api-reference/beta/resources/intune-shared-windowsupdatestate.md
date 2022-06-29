---
title: Тип ресурса windowsUpdateState
description: Тип ресурса windowsUpdateState
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1fcebd4d516d7cc91a3c33163b3325676b824b4a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444518"
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
|id|String|Это идентификатор сущности.|
|deviceId|String|Идентификатор устройства.|
|userId|String|Идентификатор пользователя.|
|deviceDisplayName|String|Отображаемое имя устройства.|
|userPrincipalName|String|Имя участника-пользователя.|
|status|[windowsUpdateStatus](/resources/intune-shared-windowsupdatestatus.md)|Состояние UDPATE Windows. Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|qualityUpdateVersion|String|Версия обновления качества устройства.|
|featureUpdateVersion|String|Текущая версия обновления компонентов устройства.|
|lastScanDateTime|DateTimeOffset|Дата, когда агент клиентский компонент Центра обновления Windows успешно сканирует.|
|lastSyncDateTime|DateTimeOffset|Время последней даты, с помощью которого устройство синхронизируется с Microsoft Intune.|

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



