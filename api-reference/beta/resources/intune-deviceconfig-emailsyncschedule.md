---
title: Тип перечисления emailSyncSchedule
description: Возможные значения для расписание синхронизации электронной почты.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc93bce19262d0b1aad1d1cc8f28ea4db56ce9f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924043"
---
# <a name="emailsyncschedule-enum-type"></a>Тип перечисления emailSyncSchedule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для расписание синхронизации электронной почты.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|asMessagesArrive|1|Синхронизация по мере поступления сообщений.|
|Вручную|2|Синхронизируйте вручную.|
|fifteenMinutes|3|Синхронизация каждые 15 минут.|
|thirtyMinutes|4|Синхронизация каждые 30 минут.|
|sixtyMinutes|5|Синхронизация каждые 60 минут.|
|basedOnMyUsage|6|Синхронизация на основе Мои использования.|





