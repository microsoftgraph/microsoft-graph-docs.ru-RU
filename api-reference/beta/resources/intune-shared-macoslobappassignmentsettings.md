---
title: тип ресурса macOsLobAppAssignmentSettings
description: Содержит свойства, используемые для назначения приложения Mac LOB группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03707af3798adabb1a1d83c789e9986c0e5076f8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068559"
---
# <a name="macoslobappassignmentsettings-resource-type"></a>тип ресурса macOsLobAppAssignmentSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения приложения Mac LOB группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|uninstallOnDeviceRemoval|Boolean|Следует ли удалить приложение при удалении устройства из Intune.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```



