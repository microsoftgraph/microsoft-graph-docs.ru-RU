---
title: тип enum emailSyncSchedule
description: Возможные значения для расписания синхронизации электронной почты.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0415b01c743c9edb3cb9f777d86c77446528d7a6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020415"
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



