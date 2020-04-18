---
title: Общие сведения об API способов проверки подлинности в Azure AD
description: Методы проверки подлинности выполняют проверку подлинности пользователей в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 73f4bb06d15c6b2e41226e872b71ba417de1076b
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557908"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Общие сведения об API способов проверки подлинности в Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (AD). Методы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которые могут управляться сегодня в Microsoft Graph, среди многих других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Методы проверки подлинности используются в основной, второй фактор и пошаговой проверке подлинности, а также в процессе самообслуживания пароля (SSPR).

API метода проверки подлинности используются для управления методами проверки подлинности пользователя. Например:

* Вы можете добавить номер телефона для пользователя. После этого пользователь может использовать этот номер телефона для проверки подлинности SMS и голосовых вызовов, если они включены для использования политикой. 
* Вы можете обновить этот номер или удалить его из пользователя.
* Вы можете включить или отключить Ввод номера для входа в SMS.
* Вы можете сбросить пароль пользователя.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Какие методы проверки подлинности могут управляться в Microsoft Graph?

|Способ проверки подлинности        | Описание |Примеры     |
|:---------------------------|:------------|:------------|
|[пассвордаусентикатионмесод](passwordauthenticationmethod.md)| В настоящее время в Azure AD используется пароль, используемый по умолчанию в качестве основного метода проверки подлинности.|Сброс пароля пользователя|
|[фонеаусентикатионмесод](phoneauthenticationmethod.md)|Пользователь может использовать телефон для проверки подлинности с помощью [SMS или голосовых вызовов](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (как это разрешено политикой).|Просмотрите номера телефонов проверки подлинности пользователя. Добавление, обновление или удаление номера телефона для пользователя. Включение или отключение основного мобильного телефона для входа в SMS.|

## <a name="next-steps"></a>Дальнейшие действия

* Изучите типы методов проверки подлинности и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
