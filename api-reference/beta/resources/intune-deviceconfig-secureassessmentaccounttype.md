---
title: secureAssessmentAccountType enum type
description: Тип учетных записей, разрешенных для Windows10SecureAssessment ConfigurationAccount.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26cea223c419260fa14256dc94a832000281fd6f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791883"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип учетных записей, разрешенных для Windows10SecureAssessment ConfigurationAccount.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|azureADAccount|0|Указывает учетную запись Azure AD в формате AzureAD\username@tenant.com.|
|domainAccount|1|Указывает учетную запись домена в формате domain\user или user@domain.com.|
|localAccount|2|Указывает локализованную учетную запись в формате имени пользователя.|
|localGuestAccount|3|Указывает локализованную учетную запись гостей в формате тестового имени.|



