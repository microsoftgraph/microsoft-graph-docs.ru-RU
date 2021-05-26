---
title: тип enum deviceManagementConfigurationTemplateFamily
description: Описывает объект TemplateFamily для объекта Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 088e1ccd80e59b95419c17d532c82c1ea9c388bc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666690"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a>тип enum deviceManagementConfigurationTemplateFamily

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает объект TemplateFamily для объекта Template

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|0|По умолчанию для семейства шаблонов, когда политика не связана с шаблоном|
|endpointSecurityAntivirus|10 |Семейство шаблонов для endpointSecurityAntivirus, которое управляет дискретной группой параметров антивируса для управляемых устройств|
|endpointSecurityDiskEncryption|11|Семейство шаблонов для endpointSecurityDiskEncryption, которое предоставляет параметры, которые актуальны для встроенного метода шифрования устройств, например FileVault или BitLocker|
|endpointSecurityFirewall|12 |Семейство шаблонов для EndpointSecurityFirewall, которое помогает настроить встроенный брандмауэр устройств для устройств с macOS и Windows 10|
|endpointSecurityEndpointDetectionAndResponse|13|Семейство шаблонов для EndpointSecurityEndpointDectionAndResponse, которое упрощает управление настройками EDR и бортовых устройств в Microsoft Defender для Endpoint|
|endpointSecurityAttackSurfaceReduction|14 |Семейство шаблонов для EndpointSecurityAttackSurfaceReduction, которое помогает уменьшить поверхности атак, минимизируя места, в которых ваша организация уязвима для киберугроз и атак|
|endpointSecurityAccountProtection|15|Семейство шаблонов для EndpointSecurityAccountProtection, облегчающего защиту удостоверений и учетных записей пользователей|
|endpointSecurityApplicationControl|16 |Семейство шаблонов для applicationControl, которое помогает уменьшить угрозы безопасности, ограничивая приложения, которые могут запускать пользователи, и код, который выполняется в ядре System Core (ядра)|




