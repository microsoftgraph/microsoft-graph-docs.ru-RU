---
title: Тип перечисления windowsAutopilotDeviceRemediationState
description: Состояние исправления устройства, указывающее, было ли изменено оборудование для устройства, зарегистрированного в Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6220236194bdb2bfbe655359cfc1d7291d90436
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210936"
---
# <a name="windowsautopilotdeviceremediationstate-enum-type"></a>Тип перечисления windowsAutopilotDeviceRemediationState

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние исправления устройства, указывающее, было ли изменено оборудование для устройства, зарегистрированного в Autopilot.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестное состояние.|
|noRemediationRequired|1|Изменение оборудования не обнаружено.|
|automaticRemediationRequired|2|На клиенте обнаружено изменение оборудования. Требуется дополнительное исправление.|
|manualRemediationRequired|3|На клиенте обнаружено изменение оборудования, которое не удалось разрешить автоматически. Требуется дополнительное исправление.|
|unknownFutureValue|4|Помечает конец известных значений перечисления и позволяет в будущем использовать дополнительные значения.|




