---
title: Тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
ms.openlocfilehash: 8454fd451f0659ff3ccad270df3414a850bee180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353377"
---
# <a name="sharingdetail-resource-type"></a>Тип ресурса sharingDetail

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сложный тип, содержащий свойства [общих](insights-shared.md) элементов. 

## <a name="json-representation"></a>Представление JSON
Ниже показано представление JSON ресурса.

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| Дата и время последнего общий файл. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.  |
| sharingSubject        | String.          | Тема, с которым предоставлен общий доступ в документе. |
| sharingType             | String.        | Определяет способ документ предоставлен общий доступ, может быть «Ссылка», «Вложения», «Группа», «Сайт».     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, общих документов.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |