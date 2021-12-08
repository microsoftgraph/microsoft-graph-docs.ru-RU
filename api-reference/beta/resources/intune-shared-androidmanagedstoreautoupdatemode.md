---
title: тип enum androidManagedStoreAutoUpdateMode
description: Приоритизация для автоматических обновлений приложений Управляемого магазина Android, установленных при назначении.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b571d8f1667d3a2eb7ccbde5bf0cefe176716a9c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337478"
---
# <a name="androidmanagedstoreautoupdatemode-enum-type"></a>тип enum androidManagedStoreAutoUpdateMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Приоритизация для автоматических обновлений приложений Управляемого магазина Android, установленных при назначении.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|default|0|Поведение обновления по умолчанию (устройство должно подключаться к Wi-Fi, заряжаться и активно не использоваться).|
|отложен|1|Обновления откладываются не более чем на 90 дней после того, как приложение устарело.|
|priority|2|Приложение обновляется как можно скорее разработчиком. Если устройство находится в сети, оно будет обновляться в течение нескольких минут.|
|unknownFutureValue|3|Неизвестный будущий режим (зарезервирован, не используется прямо сейчас).|




