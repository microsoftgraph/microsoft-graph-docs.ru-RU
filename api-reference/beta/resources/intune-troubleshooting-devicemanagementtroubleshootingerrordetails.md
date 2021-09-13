---
title: тип ресурса deviceManagementTroubleshootingErrorDetails
description: Объект, содержащий подробные сведения об ошибке и ее исправлении.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ae128466c0817dedb8e0ae435246a958967bba7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063659"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>тип ресурса deviceManagementTroubleshootingErrorDetails

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, содержащий подробные сведения об ошибке и ее исправлении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|контекст|String|Пока не задокументировано.|
|сбой|String|Пока не задокументировано.|
|failureDetails|Строка|Подробное описание того, что пошло не так.|
|исправление|Строка|Подробное описание устранения этой проблемы.|
|resources|[коллекция deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)|Ссылки на полезную документацию об этом сбое.|

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




