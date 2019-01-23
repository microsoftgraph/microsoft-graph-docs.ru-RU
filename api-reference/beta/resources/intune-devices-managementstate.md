---
title: Тип перечисления managementState
description: Состояние управления устройство в Майкрософт Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420019"
---
# <a name="managementstate-enum-type"></a>Тип перечисления managementState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние управления устройство в Майкрософт Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|управляемые|0|Устройство находится в разделе Управление|
|retirePending|1|Команда retire — отмену на устройстве и в процессе unenrolling из управления|
|retireFailed|2|Удаление команды не удалось выполнить на устройстве|
|wipePending|3|Команда очистки — отмену на устройстве и в процессе unenrolling из управления|
|wipeFailed|4|Не удалось выполнить команду очистки на устройстве|
|неработоспособные|5|Устройство работает неправильно.|
|deletePending|6|Команда Удалить является отмену на устройстве |
|retireIssued|7|Команда retire был отправлен для устройства|
|wipeIssued|8|Команда очистки был отправлен для устройства|
|wipeCanceled|9|Команда очистки для этого устройства была отменена|
|retireCanceled|10|Команда retire для этого устройства была отменена|
|Обнаружен|11|Устройство обнаружен, но не полностью зарегистрирован.|




