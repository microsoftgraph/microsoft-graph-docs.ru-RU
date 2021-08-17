---
title: тип enum diagnosticDataSubmissionMode
description: Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 42da759552f2e9a4137fb27ec90e399053f1b3f753e68f92e66f077702ed4774
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124775"
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
|Нет|1 |Данные телеметрии не отправляются из компонентов ОС. Примечание. Это значение применимо только к корпоративным и серверным устройствам. Использование этого параметра на других устройствах равно значению 1.|
|основные|2|Отправляет основные данные телеметрии.|
|расширенный|3 |Отправляет расширенные данные телеметрии, включая данные об использовании и анализах.|
|полный|4 |Отправляет полные данные телеметрии, включая диагностические данные, например состояние системы.|




