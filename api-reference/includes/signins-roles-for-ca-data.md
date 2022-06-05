---
author: besiler
ms.topic: include
ms.date: 05/11/2022
ms.localizationpriority: medium
ms.openlocfilehash: 8d04a2787953278a40bf231cb9b6db117a67ebb5
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898981"
---
<!-- markdownlint-disable MD041-->

### <a name="viewing-applied-conditional-access-ca-policies-in-sign-ins"></a>Просмотр примененных политик условного доступа (ЦС) при входе в систему
Примененные политики ЦС, перечисленные в свойстве **appliedConditionalAccessPolicies** , доступны только пользователям и приложениям с ролями, которые позволяют им считывать данные [условного доступа](../resources/appliedconditionalaccesspolicy.md). Если пользователь или приложение имеет разрешения на чтение журналов входа, но не разрешение на чтение данных условного доступа, свойство **appliedConditionalAccessPolicies** в ответе будет пропущено. Следующие роли Azure AD предоставляют пользователям разрешения на просмотр данных условного доступа:

+ Глобальный администратор
+ Глобальный читатель
+ Администратор безопасности
+ Читатель сведений о безопасности
+ Администратор условного доступа

Приложения должны иметь по крайней мере одно из следующих разрешений для просмотра объектов [appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) в журналах входа: 

+ Policy.Read.All
+ Policy.ReadWrite.ConditionalAccess
+ Policy.Read.ConditionalAccess

>**Примечание:** Пользователи Azure AD с любыми разрешениями могут читать журналы входа, в которых их пользователь является входом субъекта. Эта функция помогает пользователям выявлять непредвиденные действия в своих учетных записях. Пользователи не могут считывать данные ЦС из собственных журналов, если у них нет одного из указанных выше разрешений ЦС.
