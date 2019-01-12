---
title: Тип перечисления teamSpecialization
description: Описание варианта использования специальных для команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930287"
---
# <a name="teamspecialization-enum-type"></a>Тип перечисления teamSpecialization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Указывает, будет ли [группы](../resources/team.md) для конкретного варианта использования. Специализация каждой [группы](../resources/team.md) имеет доступ к уникальное поведение и каждый раз, нацелено на пример его использования. Значение по умолчанию — «none».

## <a name="members"></a>Элементы

| Элемент             | Значение | Описание                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Нет               | 0     | Тип для группы, которая предоставляет опыт стандартной рабочей группы по умолчанию.          |
| unknownFutureValue | 7     | Sentinel значение зарезервировано для выполнения будущее расширение перечисления. |
