---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 408e94fa12e0776d4d36fb85319ea16d4bf514e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726453"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип перечисления Локалсекуритйоптионсминимумсессионсекурити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Локалсекуритйоптионсминимумсессионсекурити

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|нуль|Отправка ответов LM & NTLM|
|requireNtmlV2SessionSecurity|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|require128BitEncryption|2|Отправлять только LM & NTLM ответы|
|ntlmV2And128BitEncryption|4|Отправлять только LM & только ответы NTLMv2.|





