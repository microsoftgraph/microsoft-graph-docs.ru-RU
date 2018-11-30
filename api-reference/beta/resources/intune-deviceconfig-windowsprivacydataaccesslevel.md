---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082575"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>Тип перечисления windowsPrivacyDataAccessLevel

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определите уровень доступа к определенной категории конфиденциальности данных Windows.
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|notConfigured|0|Уровень доступа не указан, не целей. Устройство может работать либо как и UserInControl или ForceAllow. Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.|
|forceAllow|1|Приложения смогут получить доступ к данным указанного конфиденциальности.|
|forceDeny|2|Приложения будет запрещен доступ к данным указанного конфиденциальности.|
|userInControl|3|При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.|





