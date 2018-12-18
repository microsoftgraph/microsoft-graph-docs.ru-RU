---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
author: tfitzmac
ms.openlocfilehash: 6eb1c1ea6eff28d90979da3ff998fd8442df353a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332412"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>Тип перечисления windowsPrivacyDataAccessLevel

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определите уровень доступа к определенной категории конфиденциальности данных Windows.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Уровень доступа не указан, не целей. Устройство может работать либо как и UserInControl или ForceAllow. Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.|
|forceAllow|1|Приложения смогут получить доступ к данным указанного конфиденциальности.|
|forceDeny|2|Приложения будет запрещен доступ к данным указанного конфиденциальности.|
|userInControl|3|При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.|





