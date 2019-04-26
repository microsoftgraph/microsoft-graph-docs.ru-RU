---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
ms.openlocfilehash: 898b43e054d4b0f010766aef72977d693993afdf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341428"
---
# <a name="clonableteamparts-enum-type"></a>тип перечисления Клонаблетеампартс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает, какая часть [команды](../resources/team.md) должна быть клонирована. 

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|1,1|Скопируйте список установленных приложений.|
|tabs|2|копирует вкладки в каналах.|
|settings|SP4|Копирует все параметры в группе вместе с параметрами группы ключей.|
|channels|8,5|копирует структуру канала (но не сообщения в канале).|
|members|16 |копирует участников и владельцев группы.|
