---
title: тип enum defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18063a477efdba423805e8a5410a162ce076770d37d80ae300974e5820a4fa60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152581"
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




