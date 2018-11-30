---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079616"
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

| Свойство      | Тип      | Description  |
| ------------- |-----------| -------------|
| webUrl        | String    | URL-адрес, приводя к указанного элемента. |
| id            | String    | Уникальный идентификатор элемента.           |
| type          | String    | Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem» |