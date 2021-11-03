---
title: тип ресурса androidManagedStoreAssignmentSettings
description: Содержит свойства, используемые для назначения мобильного приложения Android Managed Store группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a2afa3243cc19b016430e2b9960f6aecc349cdf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691542"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a>тип ресурса androidManagedStoreAssignmentSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения мобильного приложения Android Managed Store группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|AndroidManagedStoreAppTrackIds|Коллекция строк|ID дорожки, чтобы включить для этого назначения приложения.|
|autoUpdateMode|[AndroidManagedStoreAutoUpdateMode](../resources/intune-shared-androidmanagedstoreautoupdatemode.md)|Приоритизация автоматических обновлений для этого назначения приложения. Возможные значения: `default`, `postponed`, `priority`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ],
  "autoUpdateMode": "String"
}
```



