---
title: тип enum deviceEnrollmentType
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ac6112e63511a79ac5a64f14e916b497a949db0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755442"
---
# <a name="deviceenrollmenttype-enum-type"></a>тип enum deviceEnrollmentType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные способы добавления мобильного устройства в управление.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию, тип регистрации не был собран.|
|userEnrollment|1|Регистрация по инициативе пользователя через канал BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователей с учетной записью диспетчера регистрации устройств.|
|appleBulkWithUser|3|Массовое зачисление Apple с проблемой пользователя. (DEP, настраиваемый Apple)|
|appleBulkWithoutUser|4 |Массовое зачисление Apple без проблем пользователя. (DEP, Apple Configurator, Mobile Config)|
|windowsAzureADJoin|5 |Windows 10 Присоединиться к Azure AD.|
|windowsBulkUserless|6 |Windows 10 Массовая регистрация через ICD с сертификатом.|
|windowsAutoEnrollment|7 |Windows 10 автоматической регистрации. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8 |Windows 10 Azure AD Join.|
|windowsCoManagement|9 |Windows 10 Co-Management с помощью autoPilot или групповой политики.|
|windowsAzureADJoinUsingDeviceAuth|10 |Windows 10 Azure AD Join с помощью auth устройства.|
|appleUserEnrollment|11|Устройство, управляемое регистрацией пользователей Apple|
|appleUserEnrollmentWithServiceAccount|12 |Устройство, управляемое регистрацией пользователей Apple с учетной записью службы|




