---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912948"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>Тип перечисления diagnosticDataSubmissionMode

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|Нет|1|Данные телеметрии отправляется компоненты операционной системы. Примечание: Это значение применимо только к устройствам, enterprise и сервера. С помощью этого параметра на других устройствах эквивалентно параметру значение 1.|
|Базовая|2|Отправляет данные телеметрии для базовой.|
|Enhanced|3|Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.|
|Полный|4|Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.|



