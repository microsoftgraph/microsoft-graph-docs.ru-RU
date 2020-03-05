---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4750d5bc4da34f1e627d2b324827f78f830bb219
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526222"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип перечисления Локалсекуритйоптионсминимумсессионсекурити

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Локалсекуритйоптионсминимумсессионсекурити

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|нуль|Отправка ответов LM & NTLM|
|requireNtmlV2SessionSecurity|1 |Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|require128BitEncryption|2 |Отправлять только LM & NTLM ответы|
|ntlmV2And128BitEncryption|3 |Отправлять только LM & только ответы NTLMv2.|



