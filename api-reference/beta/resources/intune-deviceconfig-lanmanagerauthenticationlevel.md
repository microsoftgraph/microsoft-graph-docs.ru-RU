---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911996"
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





