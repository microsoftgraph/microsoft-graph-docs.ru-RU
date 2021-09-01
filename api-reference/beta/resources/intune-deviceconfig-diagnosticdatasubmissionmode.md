---
title: тип enum diagnosticDataSubmissionMode
description: Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2d4aa4818e018cecbf56f37936b84105a6162495
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791201"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>тип enum diagnosticDataSubmissionMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



