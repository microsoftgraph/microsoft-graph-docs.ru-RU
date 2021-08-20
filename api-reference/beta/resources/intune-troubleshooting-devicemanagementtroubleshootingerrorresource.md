---
title: тип ресурса deviceManagementTroubleshootingErrorResource
description: Объект, представляющий ссылку на сведения об устранении неполадок, может быть ссылкой на портал Azure или док Майкрософт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da7b75414aafcce5e221cbb5f6e0cfc0ea0209b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266795"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>тип ресурса deviceManagementTroubleshootingErrorResource

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий ссылку на сведения об устранении неполадок, может быть ссылкой на портал Azure или док Майкрософт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|text|String|Пока не задокументировано.|
|link|String|Ссылка на веб-ресурс. Может содержать любой из следующих форматтеров: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




