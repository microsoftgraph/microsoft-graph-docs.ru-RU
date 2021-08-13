---
title: тип enum clonableTeamParts
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 371f026b671f750ef67ec796d154fa3e399ac8967664466bdcb2bc498a11124c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252062"
---
# <a name="clonableteamparts-enum-type"></a>тип enum clonableTeamParts

Пространство имен: microsoft.graph



Описывает, какая часть [команды должна](../resources/team.md) быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|4 |Копирует все параметры в команде, а также параметры ключевых групп.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует членов и владельцев команды.|

