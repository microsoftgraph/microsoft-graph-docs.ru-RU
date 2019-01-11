---
title: Тип перечисления managementState
description: Состояние управления устройство в Майкрософт Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c439cf0ff830f471d2050eee81c91c6539e66d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844655"
---
# <a name="managementstate-enum-type"></a>Тип перечисления managementState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние управления устройство в Майкрософт Intune.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|управляемые|0|Устройство находится в разделе Управление|
|retirePending|1|Команда retire — отмену на устройстве и в процессе unenrolling из управления|
|retireFailed|2|Удаление команды не удалось выполнить на устройстве|
|wipePending|3|Команда очистки — отмену на устройстве и в процессе unenrolling из управления|
|wipeFailed|4|Не удалось выполнить команду очистки на устройстве|
|неработоспособные|5|Устройство работает неправильно.|
|deletePending|6|Команда Удалить является отмену на устройстве |
|retireIssued|7|Команда retire был отправлен для устройства|
|wipeIssued|8|Команда очистки был отправлен для устройства|
|wipeCanceled|9|Команда очистки для этого устройства была отменена|
|retireCanceled|10|Команда retire для этого устройства была отменена|
|Обнаружен|11|Устройство обнаружен, но не полностью зарегистрирован.|





