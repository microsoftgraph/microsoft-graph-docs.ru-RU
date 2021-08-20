---
title: secureAssessmentAccountType enum type
description: Тип учетных записей, разрешенных для Windows10SecureAssessment ConfigurationAccount.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 567de1b1d67cfb730ee5797e9c8b79f2ffe51d046dccfb8118bbcbc69ae1a6e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183045"
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
|domainAccount|1 |Указывает учетную запись домена в формате domain\user или user@domain.com.|
|localAccount|2|Указывает локализованную учетную запись в формате имени пользователя.|
|localGuestAccount|3 |Указывает локализованную учетную запись гостей в формате тестового имени.|




