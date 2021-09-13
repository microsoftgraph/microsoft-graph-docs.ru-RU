---
title: тип enum clonableTeamParts
description: 'Описывает, какая часть команды должна быть клонирована. '
ms.localizationpriority: medium
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 29ed2da8079d00576d19e94d792da0b1af423781
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109285"
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

