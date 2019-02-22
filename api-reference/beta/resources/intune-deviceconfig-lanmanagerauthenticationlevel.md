---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166572"
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
|lmNtlmV2AndNotLm|4|Отправлять только ответы LM _Амп_ NTLMv2. ОтКлонять LM|
|lmNtlmV2AndNotLmOrNtm|17:00|Отправлять только ответы LM _Амп_ NTLMv2. ОтКлонять LM _Амп_ NTLM|




