---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155561"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Тип ресурса Девицеманажементтраублешутинжеррорресаурце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|text|String|Н/Д|
|ссылка|String|Ссылка на веб-ресурс. Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}|

## <a name="relationships"></a>Отношения
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




