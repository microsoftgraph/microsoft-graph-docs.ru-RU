---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64db5eb78708a0cfa835bd695ba01b2c267fc4fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959318"
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





