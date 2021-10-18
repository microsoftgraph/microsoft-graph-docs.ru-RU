---
title: тип enum defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 14752803e22cdb991ecf9b7b93f3b01e49993efe
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451530"
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



