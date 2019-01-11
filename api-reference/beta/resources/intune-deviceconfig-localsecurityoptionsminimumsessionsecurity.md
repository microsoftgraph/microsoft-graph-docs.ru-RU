---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6912e7d3bba42364849165cceb28050ddacfae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833238"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>Тип перечисления localSecurityOptionsMinimumSessionSecurity

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Отправлять ответы LM и NTLM|
|requireNtmlV2SessionSecurity|1|Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование|
|require128BitEncryption|2|Отправлять LM и NTLM ответы|
|ntlmV2And128BitEncryption|3|Отправлять LM и NTLMv2 ответы|





