---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b979c66469ac29339045dd9d1341f85839084bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529762"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Ланманажераусентикатионлевел

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|лманднлтм|нуль|Отправка ответов LM & NTLM|
|lmNtlmAndNtlmV2|1 |Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|лманднтлмонли|2 |Отправлять только LM & NTLM ответы|
|lmAndNtlmV2|3 |Отправлять только LM & только ответы NTLMv2.|
|lmNtlmV2AndNotLm|4 |Отправлять только LM & NTLMv2 ответы. Отклонять LM|
|lmNtlmV2AndNotLmOrNtm|5 |Отправлять только LM & NTLMv2 ответы. Отклонять LM & NTLM|



