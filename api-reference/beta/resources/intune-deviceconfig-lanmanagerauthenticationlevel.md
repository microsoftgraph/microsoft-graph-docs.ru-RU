---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
author: tfitzmac
ms.openlocfilehash: fd5d63f262b9b6e9a27060725e721cb81c495a57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308745"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>Тип перечисления lanManagerAuthenticationLevel

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для LanManagerAuthenticationLevel
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|lmAndNltm|0|Отправлять ответы LM и NTLM|
|lmNtlmAndNtlmV2|1|Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование|
|lmAndNtlmOnly|2|Отправлять LM и NTLM ответы|
|lmAndNtlmV2|3|Отправлять LM и NTLMv2 ответы|
|lmNtlmV2AndNotLm|4|Отправьте LM и NTLMv2 ответы. Отказывать LM|
|lmNtlmV2AndNotLmOrNtm|5|Отправьте LM и NTLMv2 ответы. Отказ от LM и NTLM|





