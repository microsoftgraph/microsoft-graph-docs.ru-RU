---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026608"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>Тип перечисления firewallPacketQueueingMethodType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для firewallPacketQueueingMethod
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию|
|Этот параметр отключен|1|Отключение очереди пакетов|
|queueInbound|2|В очередь входящие зашифрованные пакеты|
|queueOutbound|3|Очередь расшифрован исходящих пакетов для пересылки|
|queueBoth|4|Очередь входящих и исходящих пакетов|



