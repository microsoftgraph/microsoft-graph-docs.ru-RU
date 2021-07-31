---
title: тип enum teamsAsyncOperationType
description: Типы teamsAsyncOperation. Участники будут добавлены здесь по мере поддержки дополнительных операций async.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 8d29e2230dad68c4efbdb5b6bd51a39472de8680
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665811"
---
# <a name="teamsasyncoperationtype-enum-type"></a>тип enum teamsAsyncOperationType

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Типы [teamsAsyncOperation](teamsasyncoperation.md). Участники будут добавлены здесь по мере поддержки дополнительных операций async.

## <a name="members"></a>"Участники"
В следующей таблице перечислены участники [развивающегося перечисления.](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) Для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` `teamifyGroup` `createChannel` `createChat`

| Member | Описание |
|:---------------|:----------|
|Недопустимый|Недействительным значением.|
|cloneTeam|Операция по клонированию команды.|
|archiveTeam|Операция архивации группы.|
|unarchiveTeam|Операция по восстановлению архивной группы.|
|createTeam|Операция по созданию команды с нуля.|
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |
|teamifyGroup |Операция по созданию группы из группы. |
|createChannel |Операция по созданию канала в команде. |
|createChat|Операция по созданию чата с нуля.|
