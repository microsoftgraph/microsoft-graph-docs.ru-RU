---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 670cb0bec6915b79102eae227a261f26eb052413
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790379"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Ланманажераусентикатионлевел

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|лманднлтм|нуль|Отправка ответов LM & NTLM|
|lmNtlmAndNtlmV2|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|лманднтлмонли|2|Отправлять только LM & NTLM ответы|
|lmAndNtlmV2|4|Отправлять только LM & только ответы NTLMv2.|
|lmNtlmV2AndNotLm|4 |Отправлять только LM & NTLMv2 ответы. Отклонять LM|
|lmNtlmV2AndNotLmOrNtm|5 |Отправлять только LM & NTLMv2 ответы. Отклонять LM & NTLM|



