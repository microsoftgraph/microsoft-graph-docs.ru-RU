---
title: тип enum androidManagedAppSafetyNetDeviceAttestationType
description: Требование об обязательной проверке устройств Android SafetyNet администратором в управляемом приложении.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cd8140bacc4a76b63ec4e09fe3a6ded4f535a9fe9eee59b2b6f790f2803005fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197928"
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
|basicIntegrity|1 |требуется, чтобы устройство Android прошело проверку целостности SafetyNet Basic Integrity|
|basicIntegrityAndDeviceCertification|2|требует, чтобы android-устройство проходит проверки целостности и сертификации устройств SafetyNet|




