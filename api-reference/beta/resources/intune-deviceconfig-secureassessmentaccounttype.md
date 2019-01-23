---
title: Тип перечисления secureAssessmentAccountType
description: Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409883"
---
# <a name="secureassessmentaccounttype-enum-type"></a>Тип перечисления secureAssessmentAccountType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|azureADAccount|0|Указывает учетную запись Azure AD в формате AzureAD\ username@tenant.com.|
|domainAccount|1|Указывает учетную запись домена в формате "домен\пользователь" или user@domain.com.|
|localAccount|2|Указывает локальной учетной записи в формате имя пользователя.|




