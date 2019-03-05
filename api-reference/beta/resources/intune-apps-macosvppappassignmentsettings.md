---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 102869101b577eadb40eb4a3146c45e422d9c24a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150983"
---
# <a name="macosvppappassignmentsettings-resource-type"></a>Тип ресурса Макосвппаппассигнментсеттингс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|useDeviceLicensing|Boolean|Указывает, используется ли лицензирование устройств.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```




