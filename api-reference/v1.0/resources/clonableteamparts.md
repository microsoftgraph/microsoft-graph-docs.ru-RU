---
title: Тип перечисления clonableTeamParts
description: 'Описывает, какая часть команды должна быть клонирована. '
ms.localizationpriority: medium
author: nkramer
ms.prod: teamwork
doc_type: enumPageType
ms.openlocfilehash: cf317d3487cbd4a29bb860abda4510c2223aec24
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899444"
---
# <a name="clonableteamparts-enum-type"></a>Тип перечисления clonableTeamParts

Пространство имен: microsoft.graph



Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|4|Копирует все параметры в команде вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16|копирует участников и владельцев команды.|

