---
title: тип enum localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3ecff15416ff3d313840d7b3a0ca33c2ef83e3b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033688"
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
|requireNtmlV2SessionSecurity|1|Отправить службу & NTLM-use NTLMv2 в случае переговоров|
|require128BitEncryption|2|Отправка только ответов & NTLM|
|ntlmV2And128BitEncryption|3|Отправка ответов & NTLMv2|



