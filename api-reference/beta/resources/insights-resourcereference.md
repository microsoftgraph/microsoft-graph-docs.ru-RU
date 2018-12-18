---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363622"
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