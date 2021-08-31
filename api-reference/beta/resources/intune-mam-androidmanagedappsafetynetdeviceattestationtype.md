---
title: тип enum androidManagedAppSafetyNetDeviceAttestationType
description: Требование об обязательной проверке устройств Android SafetyNet администратором в управляемом приложении.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 63b8967bdfa480f4ba8d285517e91838347b82d6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783878"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a>тип enum androidManagedAppSafetyNetDeviceAttestationType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Требование об обязательной проверке устройств Android SafetyNet администратором в управляемом приложении.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|без набора требований|
|basicIntegrity|1|требуется, чтобы устройство Android прошело проверку целостности SafetyNet Basic Integrity|
|basicIntegrityAndDeviceCertification|2|требует, чтобы android-устройство проходит проверки целостности и сертификации устройств SafetyNet|



