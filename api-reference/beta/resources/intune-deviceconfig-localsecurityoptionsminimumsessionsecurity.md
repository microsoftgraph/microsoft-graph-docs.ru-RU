---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350639"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>Тип перечисления localSecurityOptionsMinimumSessionSecurity

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Отправлять ответы LM и NTLM|
|requireNtmlV2SessionSecurity|1|Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование|
|require128BitEncryption|2|Отправлять LM и NTLM ответы|
|ntlmV2And128BitEncryption|3|Отправлять LM и NTLMv2 ответы|





