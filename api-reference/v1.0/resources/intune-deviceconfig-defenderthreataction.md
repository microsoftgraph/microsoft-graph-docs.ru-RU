---
title: Тип перечисления defenderThreatAction
description: Действие по умолчанию Защитника для обнаруженных вредоносных программ угрозы, связанные с.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976648"
---
# <a name="defenderthreataction-enum-type"></a>Тип перечисления defenderThreatAction

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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



