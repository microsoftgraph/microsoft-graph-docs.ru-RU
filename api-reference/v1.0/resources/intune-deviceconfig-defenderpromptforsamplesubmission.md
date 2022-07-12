---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса отправки примеров пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5445d9e279c1bbc98e58767d79638b0b8872ae25
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734349"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>Тип перечисления defenderPromptForSampleSubmission

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для запроса отправки примеров пользователем.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Определяемое пользователем значение по умолчанию, без намерения.|
|alwaysPrompt|1|Всегда запрашивать.|
|promptBeforeSendingPersonalData|2|Автоматически отправлять безопасные образцы.|
|neverSendData|3|Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4|Отправка всех данных без запроса.|





