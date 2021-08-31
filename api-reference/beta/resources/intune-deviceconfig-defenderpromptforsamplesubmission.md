---
title: тип enum defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя на отправку образцов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bcdb34abe2c4223bc947c15271437a2bae829372
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58751953"
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



