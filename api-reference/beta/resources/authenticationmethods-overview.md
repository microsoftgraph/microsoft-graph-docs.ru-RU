---
title: Общие сведения об API способов проверки подлинности в Azure AD
description: Методы проверки подлинности выполняют проверку подлинности пользователей в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: bb1dd599143447b597c4f57c93b20f3261ecf303
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034124"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Общие сведения об API способов проверки подлинности в Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (AD). Способы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которыми можно управлять в Microsoft Graph уже сегодня, и множество других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).

API метода проверки подлинности используются для управления методами проверки подлинности пользователя. Например:

* Вы можете добавить номер телефона для пользователя. После этого пользователь может использовать этот номер телефона для проверки подлинности SMS и голосовых вызовов, если они включены для использования политикой. 
* Вы можете обновить этот номер или удалить его из пользователя.
* Вы можете включить или отключить Ввод номера для входа в SMS.
* Вы можете сбросить пароль пользователя.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Какие методы проверки подлинности могут управляться в Microsoft Graph?

|Способ проверки подлинности        | Описание |Примеры     |
|:---------------------------|:------------|:------------|
|[пассвордаусентикатионмесод](passwordauthenticationmethod.md)| В настоящее время в Azure AD используется пароль, используемый по умолчанию в качестве основного метода проверки подлинности.|сбросить пароль пользователя.|
|[фонеаусентикатионмесод](phoneauthenticationmethod.md)|Пользователь может использовать телефон для проверки подлинности с помощью [SMS или голосовых вызовов](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (как это разрешено политикой).|Просмотрите номера телефонов проверки подлинности пользователя. Добавление, обновление или удаление номера телефона для пользователя. Включение или отключение основного мобильного телефона для входа в SMS.|

## <a name="next-steps"></a>Дальнейшие действия

* Изучите типы методов проверки подлинности и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).


