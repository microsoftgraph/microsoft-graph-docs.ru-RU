---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92cb5b32d8b4768af63d92461597c32f858c0a7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946156"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип перечисления Ланманажераусентикатионлевел

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Ланманажераусентикатионлевел

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Лманднлтм|нуль|Отправка ответов LM _Амп_ NTLM|
|lmNtlmAndNtlmV2|1,1|Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|Лманднтлмонли|2|Отправлять только LM _Амп_ NTLM ответы|
|lmAndNtlmV2|4|Отправлять только LM _Амп_ NTLMv2 ответы|
|lmNtlmV2AndNotLm|SP4|Отправлять только ответы LM _Амп_ NTLMv2. Отклонять LM|
|lmNtlmV2AndNotLmOrNtm|17:00|Отправлять только ответы LM _Амп_ NTLMv2. Отклонять LM _Амп_ NTLM|




