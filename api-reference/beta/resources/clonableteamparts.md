---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 287e63d9972043508c62b29ccf9b72d19accc337
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507658"
---
# <a name="clonableteamparts-enum-type"></a>тип перечисления Клонаблетеампартс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает, какая часть [команды](../resources/team.md) должна быть клонирована. 

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1,1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|4 |Копирует все параметры в группе вместе с параметрами группы ключей.|
|channels|8 |копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует участников и владельцев группы.|
