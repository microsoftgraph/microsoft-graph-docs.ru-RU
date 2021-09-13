---
title: брандмауэрPacketQueueingMethodType enum type
description: Возможные значения для брандмауэраPacketQueueingMethod
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fde6546255160e91d698f2a7dfe8c15c9fda26a2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139830"
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




