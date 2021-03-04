---
title: тип enum deviceEnrollmentType
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d3bc9b0862dd376b393019838980ce9c82c7df3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440173"
---
# <a name="deviceenrollmenttype-enum-type"></a>тип enum deviceEnrollmentType

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные способы добавления мобильного устройства в управление.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию, тип регистрации не был собран.|
|userEnrollment|1 |Регистрация по инициативе пользователя через канал BYOD.|
|deviceEnrollmentManager|2 |Регистрация пользователей с учетной записью диспетчера регистрации устройств.|
|appleBulkWithUser|3 |Массовое зачисление Apple с проблемой пользователя. (DEP, настраиваемый Apple)|
|appleBulkWithoutUser|4 |Массовое зачисление Apple без проблем пользователя. (DEP, Apple Configurator, Mobile Config)|
|windowsAzureADJoin|5 |Windows 10 Azure AD Join.|
|windowsBulkUserless|6 |Регистрация Windows 10 с помощью ICD с сертификатом.|
|windowsAutoEnrollment|7 |Автоматическая регистрация Windows 10. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8 |Windows 10 bulk Azure AD Join.|
|windowsCoManagement|9 |Windows 10 Co-Management с помощью автопилота или групповой политики.|
|windowsAzureADJoinUsingDeviceAuth|10 |Windows 10 Azure AD Join using Device Auth.|
|appleUserEnrollment|11|Устройство, управляемое регистрацией пользователей Apple|
|appleUserEnrollmentWithServiceAccount|12 |Устройство, управляемое регистрацией пользователей Apple с учетной записью службы|
|azureAdJoinUsingAzureVmExtension|14 |Регистрация Azure AD Join при условии обеспечения azure VM|
|AndroidEnterpriseDedicatedDevice|15 |Устройство, посвященное предприятию Android|
|AndroidEnterpriseFullyManaged|16 |Полностью управляемый Android Enterprise|
|AndroidEnterpriseCorporateWorkProfile|17 |Корпоративный профиль корпоративной работы android|




