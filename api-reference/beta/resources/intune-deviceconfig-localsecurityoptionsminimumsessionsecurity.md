---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a087c9d99164ce5c830b2d40022d7ddd99736547
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460655"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>тип перечисления Локалсекуритйоптионсминимумсессионсекурити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Локалсекуритйоптионсминимумсессионсекурити

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|нуль|Отправка ответов LM _Амп_ NTLM|
|requireNtmlV2SessionSecurity|1,1|Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании|
|require128BitEncryption|2|Отправлять только LM _Амп_ NTLM ответы|
|ntlmV2And128BitEncryption|4|Отправлять только LM _Амп_ NTLMv2 ответы|





