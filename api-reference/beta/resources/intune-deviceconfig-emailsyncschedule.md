---
title: тип enum emailSyncSchedule
description: Возможные значения для расписания синхронизации электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 899b62b78f99f362732f9b7072d3e4a48eb1fdc6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802518"
---
# <a name="emailsyncschedule-enum-type"></a>тип enum emailSyncSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для расписания синхронизации электронной почты.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение User Defined, значение по умолчанию, без намерения.|
|asMessagesArrive|1|Синхронизация по мере поступления сообщений.|
|Вручную|2|Синхронизация вручную.|
|fifteenMinutes|3|Синхронизация каждые 15 минут.|
|thirtyMinutes|4 |Синхронизация каждые тридцать минут.|
|sixtyMinutes|5 |Синхронизация каждые шестьдесят минут.|
|basedOnMyUsage|6 |Синхронизация на основе моего использования.|



