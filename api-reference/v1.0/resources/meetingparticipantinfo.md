---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742001"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса МитингпартиЦипантинфо

Пространство имен: microsoft.graph

Сведения о участниках собрания.

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| хищения | [identitySet](identityset.md) | Сведения об удостоверении участника.                                            |
| Основное      | String                        | Имя участника пользователя.                                             |
| role     | онлинемитингроле             | Указывает роль участника в собрании.  Возможные значения перечислены в следующей таблице. |

### <a name="onlinemeetingrole-values"></a>значения Онлинемитингроле

| Значение              | Описание                     |
| ------------------ | ------------------------------- |
| attendee           | Участник является участником. |
| докладчика          | Участник является выступающим. |
| unknownFutureValue | Неизвестное будущее значение.           |

## <a name="json-representation"></a>Представление JSON

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

