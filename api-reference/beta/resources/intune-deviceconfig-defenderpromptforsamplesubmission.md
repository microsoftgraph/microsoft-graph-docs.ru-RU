---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403317"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>Тип перечисления defenderPromptForSampleSubmission

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для запроса пользователя для отправки примеров.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|alwaysPrompt|1|Всегда запрашивать пользователя.|
|promptBeforeSendingPersonalData|2|Запрашивать перед отправкой личных данных.|
|neverSendData|3|Никогда не отправлять данные.|
|sendAllDataWithoutPrompting|4|Отправьте все данные без запроса.|




