---
title: тип ресурса provisionChannelEmailResult
description: Представляет результат операции по подготовка электронной почты канала.
author: anandab-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d33ebbc5e5584a8969eed6f97bf7f26042e92478
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763700"
---
# <a name="provisionchannelemailresult-resource-type"></a>тип ресурса provisionChannelEmailResult

Пространство имен: microsoft.graph

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
