---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400139"
---
# <a name="windowsupdatetype-enum-type"></a>Тип перечисления windowsUpdateType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




