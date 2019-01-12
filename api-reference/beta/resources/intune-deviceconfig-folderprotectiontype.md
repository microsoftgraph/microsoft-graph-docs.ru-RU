---
title: Тип перечисления folderProtectionType
description: Возможные значения защиты папки
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973754"
---
# <a name="folderprotectiontype-enum-type"></a>Тип перечисления folderProtectionType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения защиты папки
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение по умолчанию устройства, без цели.|
|Включение|1|Функциональные возможности блока.|
|auditMode|2|Разрешить функциональные возможности, но создать журналы.|
|blockDiskModification|3|Блокировка ненадежные приложения из записи сектора диска.|
|auditDiskModification|4|Создание журналов ненадежные приложения записи сектора диска.|





