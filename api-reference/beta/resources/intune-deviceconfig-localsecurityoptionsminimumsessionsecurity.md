---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080666"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>Тип перечисления localSecurityOptionsMinimumSessionSecurity

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|Нет|0|Отправлять ответы LM и NTLM|
|requireNtmlV2SessionSecurity|1|Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование|
|require128BitEncryption|2|Отправлять LM и NTLM ответы|
|ntlmV2And128BitEncryption|3|Отправлять LM и NTLMv2 ответы|





