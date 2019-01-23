---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416351"
---
# <a name="windowsdevicehealthstate-enum-type"></a>Тип перечисления windowsDeviceHealthState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние защиты компьютера конечной точки

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|clean|0|Компьютер чистой и никаких действий не требуется|
|fullScanPending|1|Компьютер находится в состоянии полную проверку ожидания|
|rebootPending|2|Компьютер находится в состоянии перезагрузки ожидания|
|manualStepsPending|4|Компьютер находится в состоянии ручные операции ожидания|
|offlineScanPending|8|Компьютер находится в состоянии автономной проверки ожидания|
|critical|16|Компьютер находится в состоянии критическая ошибка|




