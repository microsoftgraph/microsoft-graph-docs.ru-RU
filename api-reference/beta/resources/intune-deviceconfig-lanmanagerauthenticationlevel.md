---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801248"
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
|lmNtlmV2AndNotLm|SP4|Отправлять только ответы LM _Амп_ NTLMv2. ОтКлонять LM|
|lmNtlmV2AndNotLmOrNtm|17:00|Отправлять только ответы LM _Амп_ NTLMv2. ОтКлонять LM _Амп_ NTLM|





