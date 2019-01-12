---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 23a05a362ea57c84dceecbd9523c2620edc21fbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966288"
---
# <a name="resourcereference-resource-type"></a>Тип ресурса resourceReference

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сложный тип, содержащий свойства [средствами](insights.md).

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание  |
| ------------- |-----------| -------------|
| webUrl        | Строка    | URL-адрес, приводя к указанного элемента. |
| id            | Строка    | Уникальный идентификатор элемента.           |
| type          | Строка    | Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem» |
