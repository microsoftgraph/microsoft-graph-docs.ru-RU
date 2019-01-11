---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838971"
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



