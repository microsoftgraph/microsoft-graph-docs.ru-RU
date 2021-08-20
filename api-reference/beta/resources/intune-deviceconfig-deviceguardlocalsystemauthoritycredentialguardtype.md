---
title: тип enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 84fb6ed2690218cdecdb7a277143ba76c0a804e3776981fc45beb21a2793b70a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227466"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>тип enum deviceGuardLocalSystemAuthorityCredentialGuardType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения параметров Credential Guard.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Отключение Службы учетных данных удаленно, если настроено ранее без блокировки UEFI.|
|enableWithUEFILock|1 |Включает учетную службу с блокировкой UEFI.|
|enableWithoutUEFILock|2|Включает учетную охрану без блокировки UEFI.|
|отключение|3 |Отключает Службу учетных данных. Это значение ОС по умолчанию.|




