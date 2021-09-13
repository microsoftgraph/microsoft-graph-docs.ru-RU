---
title: тип enum lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff913766f41dfa3ec1a53c3a1ba37fc94cbc2b23
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127091"
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



