---
title: тип ресурса cloudPcWindowsSettings
description: Представляет конкретные Windows параметров для настройки при создании облачных компьютеров для политики обеспечения.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3a58fe434e73402f9d69902c58da5f20f78c5a89
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722630"
---
# <a name="cloudpcwindowssettings-resource-type"></a>тип ресурса cloudPcWindowsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конкретные Windows параметров для настройки при создании облачных компьютеров для политики обеспечения.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|language|String|Тег Windows языка и региона, который можно использовать для конфигурации языковых пакетов и локализации облачного КОМПЬЮТЕРА. Значение по умолчанию соответствует `en-US`английскому (США).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcWindowsSettings",
  "language": "String"
}
```
