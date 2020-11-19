---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7fd08d1ce3dd40e3c60c8cbc42985f4014e1f332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269030"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

Пространство имен: microsoft.graph

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




