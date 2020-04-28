---
title: Тип ресурса Девицеманажементтраублешутинжеррордетаилс
description: Объект, содержащий подробные сведения об ошибке и ее исправлении.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fd96bafac19a3501160a3aadcd830be7643f576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462267"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>Тип ресурса Девицеманажементтраублешутинжеррордетаилс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, содержащий подробные сведения об ошибке и ее исправлении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|контекст|String|Пока не задокументировано.|
|Failure|String|Пока не задокументировано.|
|фаилуредетаилс|String|Подробное описание того, что пошло не так.|
|исправления|String|Подробное описание этой проблемы.|
|resources|Коллекция [девицеманажементтраублешутинжеррорресаурце](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)|Ссылки на полезную документацию об этой ошибке.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```



