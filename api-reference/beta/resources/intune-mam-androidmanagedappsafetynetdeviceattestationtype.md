---
title: тип enum androidManagedAppSafetyNetDeviceAttestationType
description: Требование об обязательной проверке устройств Android SafetyNet администратором в управляемом приложении.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a466567752db4fe880bcb9af72b6be6625d0df4c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075272"
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



