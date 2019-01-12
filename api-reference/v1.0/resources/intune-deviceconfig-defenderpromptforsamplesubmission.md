---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e103916bd55e6c2d505a85c379b80962ab9a0cac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928089"
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



