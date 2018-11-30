---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075279"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>Тип перечисления lanManagerAuthenticationLevel

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для LanManagerAuthenticationLevel
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|lmAndNltm|0|Отправлять ответы LM и NTLM|
|lmNtlmAndNtlmV2|1|Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование|
|lmAndNtlmOnly|2|Отправлять LM и NTLM ответы|
|lmAndNtlmV2|3|Отправлять LM и NTLMv2 ответы|
|lmNtlmV2AndNotLm|4|Отправьте LM и NTLMv2 ответы. Отказывать LM|
|lmNtlmV2AndNotLmOrNtm|5|Отправьте LM и NTLMv2 ответы. Отказ от LM и NTLM|





