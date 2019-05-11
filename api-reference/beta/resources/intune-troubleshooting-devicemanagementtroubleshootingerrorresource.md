---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 712832420b556517be8ef053cc6cd292acfeed86
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939863"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Тип ресурса Девицеманажементтраублешутинжеррорресаурце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|text|String|Пока не задокументировано.|
|ссылка|Строка|Ссылка на веб-ресурс. Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}|

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




