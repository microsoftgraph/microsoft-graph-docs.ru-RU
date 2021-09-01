---
title: тип enum localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1ea1d1a0b1cb268bfa86838ec6afcb4f6751f634
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819152"
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



