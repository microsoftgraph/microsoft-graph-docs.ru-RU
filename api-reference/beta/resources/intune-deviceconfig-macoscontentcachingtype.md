---
title: тип enum macOSContentCachingType
description: Указывает тип контента, разрешенного к кэшингу службой кэшинга контента Apple.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c61a195e2b0c3025ca3659bdcfacc4075fe9367d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017480"
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



