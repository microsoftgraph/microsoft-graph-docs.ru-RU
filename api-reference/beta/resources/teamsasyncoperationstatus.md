---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075765"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>Тип перечисления teamsAsyncOperationStatus

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Description |
|:---------------|:--------|:----------|
|Недопустимый|0|Недопустимое значение.|
|notStarted|1|Эта операция не запущена.|
|inProgress|2|Выполнение операции.|
|succeeded|3|Операция успешно завершена.|
|failed|4|Сбой операции.|