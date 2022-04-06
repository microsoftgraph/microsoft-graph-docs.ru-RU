---
title: тип ресурса windowsDriverUpdateProfileInventorySyncStatus
description: Сложный тип для хранения состояния синхронизации инвентаризации профилей драйвера и прошивки. Состояние включает последнее время успешной синхронизации и состояние последней синхронизации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86bc48fd07619d7d5e99ef61239e6a92478cbd0f
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631266"
---
# <a name="windowsdriverupdateprofileinventorysyncstatus-resource-type"></a>тип ресурса windowsDriverUpdateProfileInventorySyncStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения состояния синхронизации инвентаризации профилей драйвера и прошивки. Состояние включает последнее время успешной синхронизации и состояние последней синхронизации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastSuccessfulSyncDateTime|DateTimeOffset|Последняя успешная дата и время синхронизации в UTC.|
|driverInventorySyncState|[windowsDriverUpdateProfileInventorySyncState](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstate.md)|Состояние последней синхронизации. Возможные значения: `pending`, , `success``failure`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "driverInventorySyncState": "String"
}
```




