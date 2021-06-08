---
title: тип ресурса provisionChannelEmailResult
description: Представляет результат операции по подготовка электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813253"
---
# <a name="provisionchannelemailresult-resource-type"></a>тип ресурса provisionChannelEmailResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет адрес электронной [почты, который был предусмотрен](..\api\channel-provisionemail.md) для [канала.](channel.md)

## <a name="properties"></a>Свойства
| Свойство | Тип   | Описание                               |
| :------- | :----- | :---------------------------------------- |
| email    | String | Представляет предварительный адрес электронной почты. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
