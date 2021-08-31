---
title: тип enum targetedManagedAppGroupType
description: Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 716a9e646c6e0b320869998d30f2995c65d60636
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817322"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>тип enum targetedManagedAppGroupType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает набор целевых приложений, которые могут быть одним из нескольких заранее определенных списков приложений или вручную выбранный список приложений.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|selectedPublicApps|0|Нацелить коллекцию приложений, выбранных администратором вручную.|
|allCoreMicrosoftApps|1|Целевой набор основных приложений Майкрософт (Office, Edge и т.д.).|
|allMicrosoftApps|2|Нацелить все приложения с Microsoft в качестве издателя.|
|allApps|4 |Нацелить все приложения с доступным назначением.|



