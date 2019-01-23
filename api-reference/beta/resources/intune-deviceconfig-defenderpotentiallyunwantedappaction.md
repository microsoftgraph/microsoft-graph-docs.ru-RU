---
title: Тип перечисления defenderPotentiallyUnwantedAppAction
description: Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422756"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>Тип перечисления defenderPotentiallyUnwantedAppAction

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Защита PUA отключено. Защитник будет обеспечивает защиту от нежелательных приложений.|
|блок|1|Защита от PUA включена. Обнаруженными блокируются. Они будут отображаться в журнал, а также другие угрозы, связанные с.|
|Аудит|2|Режим аудита. Защитник обнаружения нежелательных приложений, но не действий. Можно просмотреть сведения о приложениях Защитник бы вступили претензий поиск по ключевым словам для создания Защитником событий средства просмотра событий.|




