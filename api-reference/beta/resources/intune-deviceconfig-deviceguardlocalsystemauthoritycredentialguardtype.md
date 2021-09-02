---
title: тип enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c4369a5bf5752edf9c0636f31f936ecd43048407
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817112"
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
|enableWithUEFILock|1|Включает учетную службу с блокировкой UEFI.|
|enableWithoutUEFILock|2|Включает учетную охрану без блокировки UEFI.|
|отключение|3|Отключает Службу учетных данных. Это значение ОС по умолчанию.|



