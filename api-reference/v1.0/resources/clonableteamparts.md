---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
ms.openlocfilehash: d3af833dd061d6ec75b779b2ce4fe855c957f414
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027731"
---
# <a name="clonableteamparts-enum-type"></a>Тип перечисления clonableTeamParts



Описывается, какие части [группы](../resources/team.md) должны клонировании. 

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1|Скопируйте список установленных приложениях.|
|вкладки|2|Копирует вкладок между каналами.|
|settings|4|Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.|
|каналы|8|Копирует структуру канала (но не сообщения в канале).|
|members|16|Копирует участников и владельцев группы.|
