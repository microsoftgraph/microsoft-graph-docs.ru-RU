---
title: Тип ресурса connectionInfo
description: Объект connectionInfo определяет сведения о под соединении, используемые для связи с ресурсом.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137736"
---
# <a name="connectioninfo-resource-type"></a>Тип ресурса connectionInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект connectionInfo определяет локатор ресурсов, используемый для связи с ресурсом в azure AD Entitlement Management.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|Конечная точка, используемая управлением правами для связи с ресурсом пакета доступа.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```
