---
title: тип enum defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя на отправку образцов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b2c791bcd6a566e872ff7bc2fa41199e86981e138e88f4acef86b8d5e402dad3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227549"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>тип enum defenderPromptForSampleSubmission

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для запроса пользователя на отправку образцов.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение User Defined, значение по умолчанию, без намерения.|
|alwaysPrompt|1 |Всегда подсказывай.|
|promptBeforeSendingPersonalData|2|Отправка безопасных образцов автоматически.|
|neverSendData|3 |Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4 |Отправка всех данных без запроса.|




