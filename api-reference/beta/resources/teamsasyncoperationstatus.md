---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e136d043cf58480d93888374558a1be06ca9053d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914823"
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
