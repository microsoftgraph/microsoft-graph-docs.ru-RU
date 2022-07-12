---
title: Тип перечисления diagnosticDataSubmissionMode
description: Разрешите устройству отправлять диагностические данные телеметрии и данные телеметрии использования, такие как Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4befef2c9a4e447869a989aad27ddb5ca1641c44
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735119"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>Тип перечисления diagnosticDataSubmissionMode

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Разрешите устройству отправлять диагностические данные телеметрии и данные телеметрии использования, такие как Watson.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю задавать параметры.|
|none|1|Данные телеметрии не отправляются из компонентов ОС. Примечание. Это значение применимо только к корпоративным и серверным устройствам. Использование этого параметра на других устройствах эквивалентно установке значения 1.|
|Основные|2|Отправляет базовые данные телеметрии.|
|Расширенные|3|Отправляет расширенные данные телеметрии, включая данные об использовании и аналитические сведения.|
|Полный|4|Отправляет полные данные телеметрии, включая диагностические данные, например состояние системы.|





