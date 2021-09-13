---
title: тип ресурса deviceManagementTroubleshootingErrorResource
description: Объект, представляющий ссылку на сведения об устранении неполадок, может быть ссылкой на портал Azure или док Майкрософт.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 524f5615e165f32a1b67341d5066b56414404e7f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039009"
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




