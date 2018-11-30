---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
ms.openlocfilehash: 3f6d4a88ec4f0296bfd0d35f30695ddae14d4c95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074869"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>Тип перечисления firewallPreSharedKeyEncodingMethodType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для firewallPreSharedKeyEncodingMethod
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|deviceDefault|0|Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию|
|Нет|1|Предварительный ключ не кодируются. Вместо этого он будет храниться в формате Юникода|
|utF8|2|Кодирование предварительный ключ, используя UTF-8|





