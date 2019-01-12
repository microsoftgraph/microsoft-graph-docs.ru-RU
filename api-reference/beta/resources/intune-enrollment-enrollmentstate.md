---
title: Тип перечисления enrollmentState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933591"
---
# <a name="enrollmentstate-enum-type"></a>Тип перечисления enrollmentState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние регистрации устройства неизвестно|
|регистрации|1|Регистрации устройство.|
|pendingReset|2|Участвуют, но зарегистрирован посредством профиля регистрации и зарегистрированных профилей отличается от назначенного профиля.|
|failed|3|Не участвуют и запись сбоя регистрации.|
|notContacted|4|Устройство импортировать, но не участвуют.|
|заблокировано|5|Устройство участвуют как userless, но запретом переход к регистрации пользователя, так как не удается установить приложение.|





