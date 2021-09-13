---
title: тип enum deviceManagementConfigurationTemplateFamily
description: Описывает объект TemplateFamily для объекта Template
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f89437d7f9e053371698febc4867b8c384763e1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148181"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a>тип enum deviceManagementConfigurationTemplateFamily

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает объект TemplateFamily для объекта Template

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|По умолчанию для семейства шаблонов, когда политика не связана с шаблоном|
|endpointSecurityAntivirus|10 |Семейство шаблонов для endpointSecurityAntivirus, которое управляет дискретной группой параметров антивируса для управляемых устройств|
|endpointSecurityDiskEncryption|11|Семейство шаблонов для EndpointSecurityDiskEncryption, которое предоставляет параметры, которые актуальны для встроенного метода шифрования устройств, таких как FileVault или BitLocker|
|endpointSecurityFirewall|12 |Семейство шаблонов для EndpointSecurityFirewall, которое помогает настроить встроенный брандмауэр устройств для устройств с macOS и Windows 10|
|endpointSecurityEndpointDetectionAndResponse|13|Семейство шаблонов для EndpointSecurityEndpointDetectionAndResponse, которое упрощает управление настройками EDR и бортовых устройств в Microsoft Defender для endpoint|
|endpointSecurityAttackSurfaceReduction|14 |Семейство шаблонов для EndpointSecurityAttackSurfaceReduction, которое помогает уменьшить поверхности атак, минимизируя места, в которых ваша организация уязвима для киберугроз и атак|
|endpointSecurityAccountProtection|15 |Семейство шаблонов для EndpointSecurityAccountProtection, облегчающего защиту удостоверений и учетных записей пользователей|
|endpointSecurityApplicationControl|16 |Семейство шаблонов для applicationControl, которое помогает уменьшить угрозы безопасности, ограничивая приложения, которые могут запускать пользователи, и код, который выполняется в ядре System Core (ядра)|



