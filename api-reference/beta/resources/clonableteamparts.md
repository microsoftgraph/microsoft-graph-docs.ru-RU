---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: 666dc3cc60490a9a30a5e2bab0b0642c34fb5009
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034086"
---
# <a name="clonableteamparts-enum-type"></a>тип перечисления Клонаблетеампартс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1 |Скопируйте список установленных приложений.|
|tabs|2 |копирует вкладки в каналах.|
|параметры|4 |Копирует все параметры в группе вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует участников и владельцев группы.|


