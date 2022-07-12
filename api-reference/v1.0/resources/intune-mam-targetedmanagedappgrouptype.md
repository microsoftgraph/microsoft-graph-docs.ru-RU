---
title: Тип перечисления targetedManagedAppGroupType
description: Указывает коллекцию целевых приложений, которая может быть одним из нескольких предварительно определенных списков приложений или списком приложений, выбранных вручную.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e7c6dd39ff11f961f93d844a1b85f38f634ee343
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730590"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>Тип перечисления targetedManagedAppGroupType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает коллекцию целевых приложений, которая может быть одним из нескольких предварительно определенных списков приложений или списком приложений, выбранных вручную.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|selectedPublicApps|0|Выберите коллекцию приложений, выбранных администратором вручную.|
|allCoreMicrosoftApps|1|Выберите основной набор приложений Майкрософт (Office, Edge и т. д.).|
|allMicrosoftApps|2|Нацелить все приложения с корпорацией Майкрософт в качестве издателя.|
|allApps|4|Нацелить все приложения с доступным назначением.|





