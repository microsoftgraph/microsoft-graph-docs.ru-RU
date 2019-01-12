---
title: Тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: add63a89a451b742778dda1d6d313d58f675a642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918765"
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
| sharingSubject        | Строка          | Тема, с которым предоставлен общий доступ в документе. |
| sharingType             | Строка        | Определяет способ документ предоставлен общий доступ, может быть «Ссылка», «Вложения», «Группа», «Сайт».     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Пользователь, общих документов.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
