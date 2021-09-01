---
title: тип enum lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 059000a40c2d1cd1cade2a668f09c9fdaf30ee17
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58812391"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>тип enum lanManagerAuthenticationLevel

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для LanManagerAuthenticationLevel

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|lmAndNltm|0|Отправка ответов & NTLM|
|lmNtlmAndNtlmV2|1|Отправить службу & NTLM-use NTLMv2 в случае переговоров|
|lmAndNtlmOnly|2|Отправка только ответов & NTLM|
|lmAndNtlmV2|3|Отправка ответов & NTLMv2|
|lmNtlmV2AndNotLm|4 |Отправьте ответы & NTLMv2. Отказ от LM|
|lmNtlmV2AndNotLmOrNtm|5 |Отправьте ответы & NTLMv2. Отказ от LM & NTLM|



