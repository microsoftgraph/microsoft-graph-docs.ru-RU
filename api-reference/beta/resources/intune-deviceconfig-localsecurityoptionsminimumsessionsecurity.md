---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325528"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип перечисления Локалсекуритйоптионсминимумсессионсекурити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Локалсекуритйоптионсминимумсессионсекурити

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|нуль|Отправка ответов LM & NTLM|
|requireNtmlV2SessionSecurity|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|require128BitEncryption|2|Отправлять только LM & NTLM ответы|
|ntlmV2And128BitEncryption|4|Отправлять только LM & только ответы NTLMv2.|



