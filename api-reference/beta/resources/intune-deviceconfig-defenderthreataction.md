---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400272"
---
# <a name="defenderthreataction-enum-type"></a>Тип перечисления defenderThreatAction

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Применить действие на основе определения обновления.|
|clean|1|Очистите обнаруженных угроз.|
|карантин|2|Карантин обнаруженных угроз.|
|удалить|3|Удаление обнаруженных угроз.|
|Разрешить|4|Разрешить обнаруженных угроз.|
|userDefined|5|Разрешает пользователю определить действие, которое выполняется с вредоносным угроз.|
|блок|6|Блокировка обнаруженных угроз.|




