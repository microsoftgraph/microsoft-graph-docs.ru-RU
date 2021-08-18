---
title: тип enum macOSContentCachingType
description: Указывает тип контента, разрешенного к кэшингу службой кэшинга контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d97afd473185a7a25959049322a5946012d5ad207a67c0ae4e1b7c659f59534c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206601"
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
|userContentOnly|1 |Разрешить службе кэшинга контента Apple кэш данных пользователя iCloud.|
|sharedContentOnly|2|Разрешить службе кэшинга контента Apple кэш данных, не встающих под iCloud (например, обновления приложений и программного обеспечения).|




