---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 5d9121d7cbaa10260b1a7a7ce180ed7c9f37a565
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086811"
---
# <a name="clonableteamparts-enum-type"></a>тип перечисления Клонаблетеампартс

Пространство имен: microsoft.graph



Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1 |Скопируйте список установленных приложений.|
|tabs|2 |копирует вкладки в каналах.|
|settings|4 |Копирует все параметры в группе вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует участников и владельцев группы.|

