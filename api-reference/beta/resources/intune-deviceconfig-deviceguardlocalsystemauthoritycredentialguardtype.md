---
title: тип enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров Credential Guard.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 23da4e368b1fa858dc9e831ac6d4b35bc7510962
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120173"
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



