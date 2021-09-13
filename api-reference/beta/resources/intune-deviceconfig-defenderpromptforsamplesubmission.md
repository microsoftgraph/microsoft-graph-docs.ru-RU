---
title: тип enum defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя на отправку образцов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 86b8bdb6096aa9ea86f3ce202b107c27610a1ff3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091764"
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
|alwaysPrompt|1|Всегда подсказывай.|
|promptBeforeSendingPersonalData|2|Отправка безопасных образцов автоматически.|
|neverSendData|3|Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4 |Отправка всех данных без запроса.|



