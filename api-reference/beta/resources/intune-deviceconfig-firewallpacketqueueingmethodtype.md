---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9538db02afc108573338556c8899495ca9c1f26c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957797"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>Тип перечисления firewallPacketQueueingMethodType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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





