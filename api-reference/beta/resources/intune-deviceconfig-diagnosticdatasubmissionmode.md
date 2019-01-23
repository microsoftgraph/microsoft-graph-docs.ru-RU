---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422259"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>Тип перечисления diagnosticDataSubmissionMode

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Разрешить отправку данных телеметрии диагностики и использования, таких как Watson.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|none|1|Данные телеметрии отправляется компоненты операционной системы. Примечание: Это значение применимо только к устройствам, enterprise и сервера. С помощью этого параметра на других устройствах эквивалентно параметру значение 1.|
|Базовая|2|Отправляет данные телеметрии для базовой.|
|Enhanced|3|Отправляет enhanced данные телеметрии, включая данные об использовании и обмена мнениями.|
|Полный|4|Отправляет данные телеметрии полный, включая диагностические данные, такие как состояние системы.|




