---
title: тип перечисления Макосконтенткачингтипе
description: Указывает тип контента, который может кэшироваться службой кэширования контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9022b320507cc10455e2eeb3ebd3a3ca58d52f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993842"
---
# <a name="macoscontentcachingtype-enum-type"></a>тип перечисления Макосконтенткачингтипе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип контента, который может кэшироваться службой кэширования контента Apple.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|нуль|Значение, используемое по умолчанию. Будут кэшироваться данные пользователя в iCloud и данных, не являющихся iCloud.|
|усерконтентонли|1 |Разрешить службе кэширования контента Apple кэшировать данные пользователя в iCloud.|
|шаредконтентонли|2 |Разрешить службе кэширования контента Apple кэшировать данные, не относящиеся к iCloud (например, приложения и обновления программного обеспечения).|






