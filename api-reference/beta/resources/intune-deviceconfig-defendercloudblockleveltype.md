---
title: тип enum defenderCloudBlockLevelType
description: Возможные значения уровня облачного блока
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f5c600eceaa5f19ab9358906cd6c85f1226e0ad3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033730"
---
# <a name="defendercloudblockleveltype-enum-type"></a>тип enum defenderCloudBlockLevelType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения уровня облачного блока

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию, использует уровень антивирусная программа по умолчанию и обеспечивает сильное обнаружение без увеличения риска обнаружения законных файлов|
|высокая|1|High применяет высокий уровень обнаружения.|
|highPlus|2|High + использует высокий уровень и применяет меры защиты от добавления|
|zeroTolerance|3|Нулевая толерантность блокирует все неизвестные исполняемые|



