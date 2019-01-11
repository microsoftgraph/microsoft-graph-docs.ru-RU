---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1419a719ea6fb3eff3ec2a5e0cdb3722173ef6cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809746"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>Тип перечисления defenderPromptForSampleSubmission

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для запроса пользователя для отправки примеров.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|alwaysPrompt|1|Всегда запрашивать пользователя.|
|promptBeforeSendingPersonalData|2|Запрашивать перед отправкой личных данных.|
|neverSendData|3|Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4|Отправьте все данные без запроса.|



