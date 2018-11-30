---
title: Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров защиты учетных данных.
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074858"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения параметров защиты учетных данных.
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|notConfigured|0|Отключает защиты учетных данных удаленно Если ранее настроили без UEFI блокировки.|
|enableWithUEFILock|1|Включение защиты учетных данных с UEFI блокировки.|
|enableWithoutUEFILock|2|Включение защиты учетных данных без блокировки UEFI.|





