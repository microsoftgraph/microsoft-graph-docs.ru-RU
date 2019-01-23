---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396086"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>Тип перечисления localSecurityOptionsMinimumSessionSecurity

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Отправить LM & NTLM ответы|
|requireNtmlV2SessionSecurity|1|Отправлять LM & использование NTLM сеансовая безопасность NTLMv2 при согласовании|
|require128BitEncryption|2|Отправлять LM & только NTLM ответы|
|ntlmV2And128BitEncryption|3|Отправлять LM & только ответы NTLMv2|




