---
title: тип enum emailSyncSchedule
description: Возможные значения для расписания синхронизации электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ba1c5a506e5eb8eb7831794c47d73f0c7166fc876ef40acb1b023f7cd0a3860
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165772"
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
|asMessagesArrive|1 |Синхронизация по мере поступления сообщений.|
|Вручную|2|Синхронизация вручную.|
|fifteenMinutes|3 |Синхронизация каждые 15 минут.|
|thirtyMinutes|4 |Синхронизация каждые тридцать минут.|
|sixtyMinutes|5 |Синхронизация каждые шестьдесят минут.|
|basedOnMyUsage|6 |Синхронизация на основе моего использования.|




