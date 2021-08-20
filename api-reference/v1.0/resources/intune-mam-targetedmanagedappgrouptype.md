---
title: тип enum targetedManagedAppGroupType
description: Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 25821d55944d6000a050739f1b8b6f0878cadebc
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258838"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>тип enum targetedManagedAppGroupType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|selectedPublicApps|0|Нацелить коллекцию приложений, выбранных администратором вручную.|
|allCoreMicrosoftApps|1 |Целевой набор основных приложений Майкрософт (Office, Edge и т.д.).|
|allMicrosoftApps|2|Нацелить все приложения с Microsoft в качестве издателя.|
|allApps|4 |Нацелить все приложения с доступным назначением.|




