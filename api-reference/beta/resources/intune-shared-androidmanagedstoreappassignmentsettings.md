---
title: Тип ресурса Андроидманажедстореаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 040530a9f14499b964f47c6bd3f2456521b5f742
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259125"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a>Тип ресурса Андроидманажедстореаппассигнментсеттингс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|андроидманажедстореапптраккидс|Коллекция строк|Идентификаторы отслеживания, которые необходимо включить для этого назначения приложения.|

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
  ]
}
```




