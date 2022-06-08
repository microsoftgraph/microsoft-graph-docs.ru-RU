---
title: Тип перечисления clonableTeamParts
description: 'Описывает, какая часть команды должна быть клонирована. '
ms.localizationpriority: medium
doc_type: enumPageType
ms.prod: teamwork
author: nkramer
ms.openlocfilehash: 99a50eb62af486b1d5eb84ae779627bbf8509cc1
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944170"
---
# <a name="clonableteamparts-enum-type"></a>Тип перечисления clonableTeamParts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|4|Копирует все параметры в команде вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16|копирует участников и владельцев команды.|


