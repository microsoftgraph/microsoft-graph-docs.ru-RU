---
title: тип перечисления Макосконтенткачингтипе
description: Указывает тип контента, который может кэшироваться службой кэширования контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d065903190c0422380c7b15b70626ecb28dcf9c3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727486"
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





