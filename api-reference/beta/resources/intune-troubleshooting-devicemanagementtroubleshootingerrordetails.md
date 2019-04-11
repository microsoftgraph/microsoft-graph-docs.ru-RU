---
title: Тип ресурса Девицеманажементтраублешутинжеррордетаилс
description: Объект, содержащий подробные сведения об ошибке и ее исправлении.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfcbe0688836fa394237f1a25656540e401555f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796187"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>Тип ресурса Девицеманажементтраублешутинжеррордетаилс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, содержащий подробные сведения об ошибке и ее исправлении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|контекст|String|Пока не задокументировано.|
|Failure|String|Пока не задокументировано.|
|Фаилуредетаилс|String|Подробное описание того, что пошло не так.|
|исправления|String|Подробное описание этой проблемы.|
|resources|Коллекция [девицеманажементтраублешутинжеррорресаурце](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)|Ссылки на полезную документацию об этой ошибке.|

## <a name="relationships"></a>Отношения
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



