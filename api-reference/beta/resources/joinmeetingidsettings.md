---
title: Тип ресурса joinMeetingIdSettings
description: Указывает joinMeetingId, секретный код собрания и требование секретного кода.
author: yuyaolian-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fc954abe7c265c864587fdc5c2c6150c78374970
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645712"
---
# <a name="joinmeetingidsettings-resource-type"></a>Тип ресурса joinMeetingIdSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает **joinMeetingId**, секретный код собрания и требование секретного кода для собрания по сети.

## <a name="properties"></a>Свойства

| Свойство            | Тип      | Описание                                   |
|:--------------------|:----------|:----------------------------------------------|
| isPasscodeRequired  | Логическое   | Указывает, требуется ли секретный код для присоединения к собранию при использовании **joinMeetingId**. Необязательное. |
| joinMeetingId       | String    | Идентификатор собрания, используемый для присоединения к собранию. Необязательно. Только для чтения. |
| passcode            | String    | Секретный код для присоединения к собранию.  Необязательно. Только для чтения. |
## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.joinMeetingIdSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.joinMeetingIdSettings",
  "isPasscodeRequired": "Boolean",
  "joinMeetingId": "String",
  "passcode": "String"
}
```
