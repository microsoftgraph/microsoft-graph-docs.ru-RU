---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 14b991b0b00541306a47c56f8c2914c68bff07e4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734356"
---
# <a name="defendercloudblockleveltype-enum-type"></a>Тип перечисления defenderCloudBlockLevelType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения уровня облачного блока

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию, использует уровень блокировки антивирусная программа  по умолчанию и обеспечивает надежное обнаружение без повышения риска обнаружения допустимых файлов.|
|Высокой|1|Высокий уровень применяет высокий уровень обнаружения.|
|highPlus|2|High + использует высокий уровень и применяет меры защиты сложения|
|zeroTolerance|3|Нулевое погрешность блокирует все неизвестные исполняемые файлы|





