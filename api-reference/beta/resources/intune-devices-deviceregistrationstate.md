---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7633419ebeeb5c5865cd1a80c251effbf314b018
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829766"
---
# <a name="deviceregistrationstate-enum-type"></a>Тип перечисления deviceRegistrationState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние регистрации устройства.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notRegistered|0|Устройство не зарегистрирован.|
|зарегистрирована|2|Зарегистрированные устройства.|
|отменено|3|Устройства был заблокирован, очистить или не поддерживается.|
|keyConflict|4|Устройство имеет конфликты ключа.|
|approvalPending|5|Устройство ожидает утверждения.|
|certificateReset|6|Устройство сертификат был изменен.|
|notRegisteredPendingEnrollment|7|Устройства не зарегистрирована и ожидающие заявок через Интернет.|
|unknown|8|Состояние регистрации устройства неизвестно.|





