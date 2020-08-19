---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 220da0696f15fd312df9701f561f9d7c45c3e831
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808279"
---
# <a name="clonableteamparts-enum-type"></a>тип перечисления Клонаблетеампартс

Пространство имен: microsoft.graph



Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1,1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|4 |Копирует все параметры в группе вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует участников и владельцев группы.|
