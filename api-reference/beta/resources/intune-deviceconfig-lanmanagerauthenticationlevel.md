---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f76a0b685a0759a4455d8de805424ddd09758a63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970285"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Ланманажераусентикатионлевел

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Лманднлтм|нуль|Отправка ответов LM & NTLM|
|lmNtlmAndNtlmV2|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|Лманднтлмонли|2|Отправлять только LM & NTLM ответы|
|lmAndNtlmV2|4|Отправлять только LM & только ответы NTLMv2.|
|lmNtlmV2AndNotLm|SP4|Отправлять только LM & NTLMv2 ответы. Отклонять LM|
|lmNtlmV2AndNotLmOrNtm|17:00|Отправлять только LM & NTLMv2 ответы. Отклонять LM & NTLM|





