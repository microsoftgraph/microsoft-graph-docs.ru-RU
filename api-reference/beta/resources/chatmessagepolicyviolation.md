---
title: тип ресурса chatMessagePolicyViolation
description: Представляет нарушение политики в сообщении чата. Нарушения политики обычно устанавливаются приложением для предотвращения потери данных (DLP).
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9c65b6dd1d07db43286a8cf9923f4a94f0855b34
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582272"
---
# <a name="chatmessagepolicyviolation-resource-type"></a>тип ресурса chatMessagePolicyViolation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет нарушение политики в сообщении чата. Нарушения политики обычно устанавливаются приложением для предотвращения потери данных (DLP). Приложения DLP отслеживают чаты для сообщений, содержащих данные, которые не должны отправляться пользователями.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|dlpAction|**chatMessagePolicyViolationDlpActionType**|Действия, принятые поставщиком DLP в сообщении с конфиденциальным контентом. Поддерживаемые значения: <li>Нет</li><li>NotifySender . Информируйте отправитель о нарушении, но позвольте читателям прочитать сообщение.</li><li>BlockAccess . Блокировать чтение сообщения читателями.</li><li>BlockAccessExternal . Блокировать чтение сообщения пользователями за пределами организации, позволяя пользователям в организации читать сообщение.</li>|
|justificationText|string|Текст обоснования, предоставляемый отправитель сообщения при переопределения нарушения политики.|
|policyTip|[chatMessagePolicyViolationPolicyTip](chatmessagepolicyviolationpolicytip.md)|Сведения для отображения отправилю сообщения о том, почему сообщение было помечено как нарушение. |
|userAction|**chatMessagePolicyViolationUserActionType**|Указывает действие пользователя на сообщение, заблокированное поставщиком DLP. Поддерживаемые значения: <li>Нет</li><li>Override</li><li>ReportFalsePositive</li>Когда поставщик DLP обновляет сообщение для блокировки конфиденциального контента, userAction не требуется.|
|verdictDetails|**chatMessagePolicyViolationVerdictDetailsType**|Указывает, какие действия может принять отправитель в ответ на нарушение политики. Поддерживаемые значения: <li>Нет</li><li>AllowFalsePositiveOverride — позволяет отправителю объявить политикуViolation ошибкой в приложении DLP и его правилах, а также разрешить читателям снова видеть сообщение, если dlpAction его спрятал.</li><li>AllowOverrideWithoutJustification — позволяет отправителю перезахотрить нарушение DLP и разрешить читателям видеть сообщение снова, если dlpAction спрятал его, не ая при этом объяснений. </li><li>AllowOverrideWithJustification — позволяет отправителю перезахотрить нарушение DLP и разрешить читателям снова видеть сообщение, если dlpAction спрятал его, после предоставления объяснений для этого.</li>AllowOverrideWithoutJustification и AllowOverrideWithJustification являются взаимоисключающими.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
