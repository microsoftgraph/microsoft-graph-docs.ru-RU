---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397458"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>Тип перечисления lanManagerAuthenticationLevel

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для LanManagerAuthenticationLevel

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|lmAndNltm|0|Отправить LM & NTLM ответы|
|lmNtlmAndNtlmV2|1|Отправлять LM & использование NTLM сеансовая безопасность NTLMv2 при согласовании|
|lmAndNtlmOnly|2|Отправлять LM & только NTLM ответы|
|lmAndNtlmV2|3|Отправлять LM & только ответы NTLMv2|
|lmNtlmV2AndNotLm|4|Отправьте LM & только ответы NTLMv2. Отказывать LM|
|lmNtlmV2AndNotLmOrNtm|5|Отправьте LM & только ответы NTLMv2. Отказ от LM & NTLM|




