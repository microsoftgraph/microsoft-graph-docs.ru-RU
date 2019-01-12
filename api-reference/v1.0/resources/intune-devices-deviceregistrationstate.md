---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911898"
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



