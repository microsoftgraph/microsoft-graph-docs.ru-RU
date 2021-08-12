---
title: брандмауэрPacketQueueingMethodType enum type
description: Возможные значения для брандмауэраPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 77a1c26591fe529e1ec256351fb5397e96143d9b8d79eeba6b6781ca960fefa0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202407"
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




