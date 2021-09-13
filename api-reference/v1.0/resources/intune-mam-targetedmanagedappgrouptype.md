---
title: тип enum targetedManagedAppGroupType
description: Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c51f6af9c775fd1cc3010060d2ff227585d83747
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098687"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>тип enum targetedManagedAppGroupType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|selectedPublicApps|0|Нацелить коллекцию приложений, выбранных администратором вручную.|
|allCoreMicrosoftApps|1|Целевой набор основных приложений Майкрософт (Office, Edge и т.д.).|
|allMicrosoftApps|2|Нацелить все приложения с Microsoft в качестве издателя.|
|allApps|4 |Нацелить все приложения с доступным назначением.|




