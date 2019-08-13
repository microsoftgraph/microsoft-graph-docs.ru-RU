---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eaf3cc39efb52bb7f603c636a69d13e3d025ce5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347740"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Тип ресурса Девицеманажементтраублешутинжеррорресаурце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|text|String|Пока не задокументировано.|
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



