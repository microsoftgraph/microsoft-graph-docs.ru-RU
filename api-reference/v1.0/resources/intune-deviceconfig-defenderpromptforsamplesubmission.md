---
title: тип enum defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя на отправку образцов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e029792e19bb65fcf4ea6c8207cdeb511ae025eb
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455578"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>тип enum defenderPromptForSampleSubmission

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для запроса пользователя на отправку образцов.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение User Defined, значение по умолчанию, без намерения.|
|alwaysPrompt|1|Всегда подсказывай.|
|promptBeforeSendingPersonalData|2|Отправка безопасных образцов автоматически.|
|neverSendData|3|Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4 |Отправка всех данных без запроса.|



