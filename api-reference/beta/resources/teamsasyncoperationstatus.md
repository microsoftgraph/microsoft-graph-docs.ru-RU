---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332006"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>Тип перечисления teamsAsyncOperationStatus

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Недопустимый|0|Недопустимое значение.|
|notStarted|1|Эта операция не запущена.|
|inProgress|2|Выполнение операции.|
|succeeded|3|Операция успешно завершена.|
|failed|4|Сбой операции.|