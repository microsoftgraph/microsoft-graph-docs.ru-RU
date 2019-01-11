---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15d2d46684d38b57690cc9c12d9c49eccd652e6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887040"
---
# <a name="windowsupdatetype-enum-type"></a>Тип перечисления windowsUpdateType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Какие устройства филиала будет получать обновления из
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|all|1|Разделитель годовая канала (целевой). Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).|
|businessReadyOnly|2|Разделитель годовая канала. Устройства получает обновления компонента точками годовая канала.|
|windowsInsiderBuildFast|3|Построение изнутри Windows - Fast|
|windowsInsiderBuildSlow|4|Построение изнутри Windows - снижение производительности|
|windowsInsiderBuildRelease|5|Построение выпуска Windows изнутри|





