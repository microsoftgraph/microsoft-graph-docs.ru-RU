---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635200"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса МитингпартиЦипантинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о участнике собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| хищения | [identitySet](identityset.md) | Сведения об удостоверении участника.                                           |
| Основное      | String                        | Имя участника пользователя.                                            |
| role     | онлинемитингроле             | Указывает роль участника в собрании.  Возможные значения: `attendee`, `presenter` и `unknownFutureValue`.|

### <a name="onlinemeetingrole-values"></a>значения Онлинемитингроле

| Значение              | Описание                     |
| ------------------ | ------------------------------- |
| attendee           | Участник является участником. |
| докладчика          | Участник является выступающим. |
| unknownFutureValue | Неизвестное будущее значение.           |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


