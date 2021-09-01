---
title: брандмауэрPacketQueueingMethodType enum type
description: Возможные значения для брандмауэраPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b496651cb8735a06afd5ae68e56e4078095180dc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817105"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>брандмауэрPacketQueueingMethodType enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



