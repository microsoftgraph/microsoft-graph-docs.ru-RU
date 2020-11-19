---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07d284f778dd2cb5bfc9942a649aecbc63ac1b19
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269023"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип перечисления Локалсекуритйоптионсминимумсессионсекурити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Локалсекуритйоптионсминимумсессионсекурити

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|нуль|Отправка ответов LM & NTLM|
|requireNtmlV2SessionSecurity|1,1|Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|require128BitEncryption|2|Отправлять только LM & NTLM ответы|
|ntlmV2And128BitEncryption|4|Отправлять только LM & только ответы NTLMv2.|




