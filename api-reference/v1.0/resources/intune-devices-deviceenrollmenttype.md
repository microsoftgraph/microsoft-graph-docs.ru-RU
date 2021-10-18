---
title: тип enum deviceEnrollmentType
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa44fddf18daae371c7ed7fe0a9784bf0c0cc361
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455842"
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
|windowsAzureADJoin|5|Windows 10 Присоединиться к Azure AD.|
|windowsBulkUserless|6 |Windows 10 Массовая регистрация через ICD с сертификатом.|
|windowsAutoEnrollment|7 |Windows 10 автоматической регистрации. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8 |Windows 10 Azure AD Join.|
|windowsCoManagement|9 |Windows 10 Co-Management с помощью autoPilot или групповой политики.|
|windowsAzureADJoinUsingDeviceAuth|10 |Windows 10 Azure AD Join с помощью auth устройства.|
|appleUserEnrollment|11|Устройство, управляемое регистрацией пользователей Apple|
|appleUserEnrollmentWithServiceAccount|12 |Устройство, управляемое регистрацией пользователей Apple с учетной записью службы|



