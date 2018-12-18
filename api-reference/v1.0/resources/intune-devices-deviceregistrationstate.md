---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
ms.openlocfilehash: 9fdd5cd3a63472e841f0d97f8cbee3a0f548380d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320093"
---
# <a name="deviceregistrationstate-enum-type"></a>Тип перечисления deviceRegistrationState

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



