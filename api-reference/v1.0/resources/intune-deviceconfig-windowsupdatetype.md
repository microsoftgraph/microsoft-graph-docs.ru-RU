---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d1f946dd497e650df5eb07004560dda028e14f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930343"
---
# <a name="windowsupdatetype-enum-type"></a>Тип перечисления windowsUpdateType

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



