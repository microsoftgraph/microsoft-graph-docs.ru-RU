---
title: тип enum defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755891"
---
# <a name="defendercloudblockleveltype-enum-type"></a>тип enum defenderCloudBlockLevelType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения уровня облачного блока

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию, использует уровень антивирусная программа по умолчанию и обеспечивает сильное обнаружение без увеличения риска обнаружения законных файлов|
|высокая|1|High применяет высокий уровень обнаружения.|
|highPlus|2|High + использует высокий уровень и применяет меры защиты от добавления|
|zeroTolerance|3|Нулевая толерантность блокирует все неизвестные исполняемые|




