---
title: Тип ресурса Акцессревиевинстанце
description: Представляет повторение объекта `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 480774950e2257b7af099c02cbe7c6571c0ce4c6
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001070"
---
# <a name="accessreviewinstance-resource-type"></a>Тип ресурса Акцессревиевинстанце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет повторение [проверки доступа](accessreviewsv2-root.md) Azure AD. Если родительская [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) — это повторяющаяся проверка доступа, экземпляры представляют каждое повторение. Проверка, которая не повторяется, будет иметь ровно один экземпляр. Экземпляры также представляют каждую уникальную группу, которая просматривается в определении расписания. Если в определении расписания просматриваются несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.

Каждый **акцессревиевинстанце** содержит список [решений](accessreviewinstancedecisionitem.md) , на которые могут выполнять действия проверяющих. Для рассмотрения одного и того же удостоверения существует одно решение.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список Акцессревиевинстанцес](../api/accessreviewinstance-list.md) | Коллекция [акцессревиевинстанце](accessreviewinstance.md) | Получение списка объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) и их свойств. |
|[Получение Акцессревиевинстанце](../api/accessreviewinstance-get.md) | [акцессревиевинстанце](accessreviewinstance.md) | Возвращает Акцессревиевинстанце для Акцессревиевсчедуледефинитион. Не включает в объект связанное АкцессревиевинстанцедеЦисионитем. |
|[Список Пендингакцессревиевинстанцес](../api/accessreviewinstance-pendingaccessreviewinstances.md) | Коллекция [акцессревиевинстанце](accessreviewinstance.md) . | Получение всех ожидающих Акцессревиевинстанце ресурсов, назначенных вызывающему пользователю. |
|[Отправка напоминания о Акцессревиевинстанце](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам Акцессревиевинстанце. |
|[Остановить Акцессревиевинстанце](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите Акцессревиевинстанце. |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызывающему пользователю принимать рекомендации по решению для каждого Нотревиевед АкцессревиевинстанцедеЦисионитем, на которые они пересматриваются для определенного Акцессревиевинстанце. |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применяйте решение для Акцессревиевинстанце. |



## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------------------------------- | :---------- |
| id | Строка | Уникальный идентификатор экземпляра. |
| displayName | Строка | Имя родительского Акцессревиевсчедуледефинитион. |
| startDateTime | DateTimeOffset | DateTime при запланированном запуске проверки экземпляра. Может быть в будущем. |
| endDateTime | DateTimeOffset | DateTime при запланированном окончании проверки экземпляра. |
| status | string | Указывает состояние Акцессревиев. Типичные состояния:,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` , `AutoReviewing` и `AutoReviewed` .  Только для чтения.|
| scope | [акцессревиевскопе](accessreviewscope.md) | Создается на основе **области действия** и **Инстанцеенумератионскопе** на уровне акцессревиевсчедуледефинитион. Определяет область пользователей, проверенных в группе. В случае с проверкой одной группы область, определенная на `accessReviewScheduleDefinition` уровне, применяется ко всем экземплярам. В случае проверки всех групп область может различаться для каждой группы. Только для чтения.  | 
| решения | Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) | Каждый пользователь, который просматривается в Акцессревиевинстанце, имеет элемент принятия решений, который представляет, был ли их доступ утвержден, отклонен или еще не проверен. |
| RDLC |[акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | С каждым экземпляром связан ровно один Акцессревиевсчедуледефинитион. Это родительское расписание для экземпляра, в котором экземпляры создаются для каждого повторения определения проверки и каждая группа, выбранная для просмотра определением. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `definition`               |[акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md)          | `accessReviewScheduleDefinition`С каждым экземпляром связан только один экземпляр. Это родительское расписание для экземпляра, в котором экземпляры создаются для каждого повторения определения проверки и каждая группа, выбранная для просмотра определением. |
| `decisions`               |Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md)        | Каждый пользователь, проверенный в элементе, `accessReviewInstance` имеет элемент принятия решений, который представляет, было ли оно утверждено, отклонено или еще не проверено. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
