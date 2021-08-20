---
title: тип enum localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b16a4a3e1e98612af7a69b63a02fcdd681d4fa7842134681603b54abcf33e648
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54136312"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип enum localSecurityOptionsMinimumSessionSecurity

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Отправка ответов & NTLM|
|requireNtmlV2SessionSecurity|1 |Отправить службу & NTLM-use NTLMv2 в случае переговоров|
|require128BitEncryption|2|Отправка только ответов & NTLM|
|ntlmV2And128BitEncryption|3 |Отправка ответов & NTLMv2|




