---
title: тип enum macOSContentCachingType
description: Указывает тип контента, разрешенного к кэшингу службой кэшинга контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0bb0859eb7b409849341b03f51abb838c62f2a18
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783542"
---
# <a name="macoscontentcachingtype-enum-type"></a>тип enum macOSContentCachingType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип контента, разрешенного к кэшингу службой кэшинга контента Apple.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение, используемое по умолчанию. Кэшировали как данные пользователя iCloud, так и данные без iCloud.|
|userContentOnly|1|Разрешить службе кэшинга контента Apple кэш данных пользователя iCloud.|
|sharedContentOnly|2|Разрешить службе кэшинга контента Apple кэш данных, не встающих под iCloud (например, обновления приложений и программного обеспечения).|



