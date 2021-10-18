---
title: тип enum diagnosticDataSubmissionMode
description: Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cc92f564c323d3a0d7303b1074c523f158a96979
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445140"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>тип enum diagnosticDataSubmissionMode

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю установить.|
|Нет|1|Данные телеметрии не отправляются из компонентов ОС. Примечание. Это значение применимо только к корпоративным и серверным устройствам. Использование этого параметра на других устройствах равно значению 1.|
|основные|2|Отправляет основные данные телеметрии.|
|расширенный|3|Отправляет расширенные данные телеметрии, включая данные об использовании и анализах.|
|полный|4 |Отправляет полные данные телеметрии, включая диагностические данные, например состояние системы.|



