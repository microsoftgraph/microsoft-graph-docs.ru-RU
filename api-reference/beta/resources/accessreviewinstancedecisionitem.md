---
title: Тип ресурса АкцессревиевинстанцедеЦисионитем
description: Представляет решение для доступа пользователя в Акцессревиевинстанце.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001067"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Тип ресурса АкцессревиевинстанцедеЦисионитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет решение по [проверке доступа](accessreviewsv2-root.md) Azure AD для экземпляра проверки. Это решение представляет определение доступа пользователя или субъекта к данному [экземпляру проверки доступа](accessreviewinstance.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список АкцессревиевинстанцедеЦисионитемс](../api/accessreviewinstancedecisionitem-list.md) | Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) | Перечисление всех АкцессревиевинстанцедеЦисионитем для определенного Акцессревиевинстанце. |
|[Список ожидающих утверждения АкцессревиевинстанцедеЦисионитемс](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) . | Получение всех АкцессревиевинстанцедеЦисионитемс, назначенных вызывающему пользователю для определенного Акцессревиевинстанце. |
|[Обновление АкцессревиевинстанцедеЦисионитем](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для всех АкцессревиевинстанцедеЦисионитемс, для которых вызывающему пользователю назначен проверяющий, вызывающий пользователь может записать решение, заменив исправление объекта принятия решений. |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
| id | Строка | Идентификатор решения. |
| акцессревиевид | Строка | Идентификатор родителя Акцессревиевинстанце. |
| ревиеведби | [userIdentity](useridentity.md) | Идентификатор проверяющего. |
| ревиеведдатетиме | DateTimeOffset | Дата и время, когда произошла проверка. |
| решении | Строка | Результат проверки. Возможные значения: `Approve` , `Deny` , `NotReviewed` , или `DontKnow` . |
| текста | Строка | Проверка обоснования решения. |
| апплиедби | [userIdentity](useridentity.md) | Идентификатор пользователя, который применил решение. |
| апплиеддатетиме | DateTimeOffset | Дата и время, когда было применено решение об утверждении. |
| апплиресулт | Строка | Результат применения решения. Возможные значения: `NotApplied` , `Success` , `Failed` , `NotFound` , или `NotSupported` . |
| Рекомендуемые | Строка | Созданная системой рекомендация для решения об утверждении. Возможные значения: `Approve` , `Deny` , или `NotAvailable` .  |
| target | [акцессревиевинстанцедеЦисионитемтаржет](accessreviewinstancedecisionitemtarget.md)  | Цель этого конкретного решения. Целевые показатели решений могут принадлежать разным типам — каждый из них имеет собственные конкретные свойства. Обратитесь к разделу [акцессревиевинстанцедеЦисионитемтаржет](accessreviewinstancedecisionitemtarget.md). |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| вхождения |[акцессревиевинстанце](accessreviewinstance.md) | Каждое решение имеет только один Акцессревиевинстанце, связанный с каждым из них. Экземпляр является родительским элементом решения, представляющим повторение проверки доступа, над которой принимается решение. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
