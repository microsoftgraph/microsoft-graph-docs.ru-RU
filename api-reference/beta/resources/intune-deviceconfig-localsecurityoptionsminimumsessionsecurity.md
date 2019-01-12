---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952484"
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





