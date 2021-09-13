---
title: secureAssessmentAccountType enum type
description: Тип учетных записей, разрешенных для Windows10SecureAssessment ConfigurationAccount.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3c7d5577c322db4f980c008f3fbc72d4756733a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081236"
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



