---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304559"
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



