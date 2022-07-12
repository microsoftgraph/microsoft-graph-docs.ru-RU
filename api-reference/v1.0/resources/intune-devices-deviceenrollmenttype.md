---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a53c4fadbce9703e4e68b54a86cfff80e1bd3944
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735371"
---
# <a name="deviceenrollmenttype-enum-type"></a>Тип перечисления deviceEnrollmentType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные способы добавления мобильного устройства в управление.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию, тип регистрации не был собран.|
|userEnrollment|1|Регистрация, управляемая пользователем, через канал BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователей с помощью учетной записи диспетчера регистрации устройств.|
|appleBulkWithUser|3|Массовая регистрация Apple с запросом пользователя. (DEP, Apple Configurator)|
|appleBulkWithoutUser|4|Массовая регистрация Apple без запроса пользователя. (DEP, Apple Configurator, Mobile Config)|
|windowsAzureADJoin|5|Windows 10 Azure AD join.|
|windowsBulkUserless|6 |Windows 10 массовой регистрации через ICD с помощью сертификата.|
|windowsAutoEnrollment|7 |Windows 10 автоматической регистрации. (Добавление рабочей учетной записи)|
|windowsBulkAzureDomainJoin|8 |Windows 10 массовое Azure AD join.|
|windowsCoManagement|9 |Windows 10 Co-Management с помощью AutoPilot или групповая политика.|
|windowsAzureADJoinUsingDeviceAuth|10|Windows 10 Azure AD присоединение с использованием проверки подлинности устройства.|
|appleUserEnrollment|11|Устройство, управляемое регистрацией пользователей Apple|
|appleUserEnrollmentWithServiceAccount|12 |Устройство, управляемое регистрацией пользователей Apple с помощью учетной записи службы|





