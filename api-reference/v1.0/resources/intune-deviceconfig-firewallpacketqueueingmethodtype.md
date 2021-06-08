---
title: брандмауэрPacketQueueingMethodType enum type
description: Возможные значения для брандмауэраPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a56e30f8b470271ea5fbb91765f7ea6814cbba14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758857"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>брандмауэрPacketQueueingMethodType enum type

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для брандмауэраPacketQueueingMethod

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства|
|отключено|1|Отключение очередей пакетов|
|queueInbound|2|Входящие в очередь зашифрованные пакеты|
|queueOutbound|3|Расшифровка исходящие пакеты очереди для переададровки|
|queueBoth|4 |Очередь как входящие, так и исходящие пакеты|




