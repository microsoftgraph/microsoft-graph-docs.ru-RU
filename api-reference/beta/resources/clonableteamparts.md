---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860559"
---
# <a name="clonableteamparts-enum-type"></a>Тип перечисления clonableTeamParts

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывается, какие части [группы](../resources/team.md) должны клонировании. 

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1|Скопируйте список установленных приложениях.|
|вкладки|2|Копирует вкладок между каналами.|
|settings|4|Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.|
|каналы|8|Копирует структуру канала (но не сообщения в канале).|
|members|16|Копирует участников и владельцев группы.|
