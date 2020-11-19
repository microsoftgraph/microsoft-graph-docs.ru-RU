---
title: тип перечисления Макосконтенткачингтипе
description: Указывает тип контента, который может кэшироваться службой кэширования контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a79cd14a6bd765f260439a259c63106e6211cacc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268736"
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
|усерконтентонли|1,1|Разрешить службе кэширования контента Apple кэшировать данные пользователя в iCloud.|
|шаредконтентонли|2|Разрешить службе кэширования контента Apple кэшировать данные, не относящиеся к iCloud (например, приложения и обновления программного обеспечения).|




