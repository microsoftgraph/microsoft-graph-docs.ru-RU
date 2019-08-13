---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356727"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Ланманажераусентикатионлевел

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|лманднлтм|нуль|Отправка ответов LM & NTLM|
|lmNtlmAndNtlmV2|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|лманднтлмонли|2|Отправлять только LM & NTLM ответы|
|lmAndNtlmV2|4|Отправлять только LM & только ответы NTLMv2.|
|lmNtlmV2AndNotLm|SP4|Отправлять только LM & NTLMv2 ответы. Отклонять LM|
|lmNtlmV2AndNotLmOrNtm|17:00|Отправлять только LM & NTLMv2 ответы. Отклонять LM & NTLM|



