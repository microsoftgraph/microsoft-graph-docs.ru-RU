---
title: Тип перечисления emailSyncSchedule
description: Возможные значения для расписание синхронизации электронной почты.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425185"
---
# <a name="emailsyncschedule-enum-type"></a>Тип перечисления emailSyncSchedule

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для расписание синхронизации электронной почты.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|asMessagesArrive|1|Синхронизация по мере поступления сообщений.|
|Вручную|2|Синхронизируйте вручную.|
|fifteenMinutes|3|Синхронизация каждые 15 минут.|
|thirtyMinutes|4|Синхронизация каждые 30 минут.|
|sixtyMinutes|5|Синхронизация каждые 60 минут.|
|basedOnMyUsage|6|Синхронизация на основе Мои использования.|




