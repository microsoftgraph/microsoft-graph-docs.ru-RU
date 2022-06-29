---
title: Назначение, обновление или удаление настраиваемых атрибутов безопасности (предварительная версия)
description: Узнайте, как назначать, обновлять или удалять настраиваемые атрибуты безопасности для пользователей и приложений (субъектов-служб) с помощью microsoft API Graph.
author: rolyon
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: directory-management
ms.openlocfilehash: 21db29dc53c3b005dd0fa09c5e13bd7cfa055a1f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442129"
---
# <a name="assign-update-or-remove-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>Назначение, обновление или удаление настраиваемых атрибутов безопасности с помощью microsoft API Graph (предварительная версия)

> [!IMPORTANT]
> Функция настраиваемых атрибутов безопасности в настоящее время находится на этапе предварительной версии. Дополнительные условия использования предварительных версий [Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) см. в юридических условиях, применимых к функциям Azure, которые находятся в бета-версии, предварительной версии или еще не выпущены в общедоступной версии.

[Настраиваемые](/azure/active-directory/fundamentals/custom-security-attributes-overview) атрибуты безопасности в Azure Active Directory (Azure AD) — это атрибуты для бизнеса (пары "ключ -значение"), которые можно определять и назначать Azure AD объектам.

В этой статье приведены примеры назначения, обновления или удаления различных типов настраиваемых атрибутов безопасности для пользователей и приложений (субъектов-служб). Настраиваемые атрибуты безопасности можно назначать `PATCH` или обновлять только с помощью операции в запросе update [user](/graph/api/user-update) [или Update servicePrincipal](/graph/api/serviceprincipal-update) .

## <a name="permissions"></a>Разрешения

Для управления настраиваемыми атрибутами безопасности вызывающему субъекту должна быть назначена Azure AD роли. По умолчанию глобальный администратор и другие роли администратора не имеют разрешений на чтение, определение или назначение настраиваемых атрибутов безопасности.

- [Администратор назначения атрибутов](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

Кроме того, вызывающему субъекту должны быть предоставлены следующие разрешения.

- [CustomSecAttributeAssignment.ReadWrite.All](permissions-reference.md#custom-security-attributes-permissions)
- [User.Read.All](permissions-reference.md#user-permissions)

Разрешения на чтение, назначение, обновление или удаление атрибутов для приложения предоставляются *customSecAttributeAssignment.ReadWrite.All*. Разрешения на чтение объекта ресурса, например пользователей, предоставляются отдельно с помощью разрешений объекта ресурса, таких как *User.Read.All*.

## <a name="assign-custom-security-attributes"></a>Назначение настраиваемых атрибутов безопасности

### <a name="example-1-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>Пример 1. Назначение пользовательского атрибута безопасности со строковым значением пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности со строковым значением.

- Набор атрибутов: `Engineering`
- Атрибут: `ProjectDate`
- Тип данных атрибута: строка
- Значение атрибута: `"2022-10-01"`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-assign-a-custom-security-attribute-with-a-string-value-to-a-service-principal"></a>Пример 2. Назначение настраиваемого атрибута безопасности со строковым значением субъекту-службе

В следующем примере показано, как назначить субъекту-службе настраиваемый атрибут безопасности со строковым значением.

- Набор атрибутов: `Engineering`
- Атрибут: `ProjectDate`
- Тип данных атрибута: строка
- Значение атрибута: `"2022-10-01"`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_serviceprincipal_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-3-assign-a-custom-security-attribute-with-a-multi-string-value-to-a-user"></a>Пример 3. Назначение пользовательского атрибута безопасности с многостроковым значением пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с многостроковым значением.

- Набор атрибутов: `Engineering`
- Атрибут: `Project`
- Тип данных атрибута: коллекция строк
- Значение атрибута: `["Baker","Cascade"]`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multistring"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project@odata.type":"#Collection(String)",
            "Project":["Baker","Cascade"]
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-4-assign-a-custom-security-attribute-with-an-integer-value-to-a-user"></a>Пример 4. Назначение пользовательского атрибута безопасности с целочисленным значением пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с целочисленным значением.

- Набор атрибутов: `Engineering`
- Атрибут: `NumVendors`
- Тип данных атрибута: Целое число
- Значение атрибута: `4`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":4
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-5-assign-a-custom-security-attribute-with-a-multi-integer-value-to-a-user"></a>Пример 5. Назначение пользовательского атрибута безопасности с несколькими целочисленными значениями пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с много целочисленным значением.

- Набор атрибутов: `Engineering`
- Атрибут: `CostCenter`
- Тип данных атрибута: коллекция целых чисел
- Значение атрибута: `[1001,1003]`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multiinteger"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "CostCenter@odata.type":"#Collection(Int32)",
            "CostCenter":[1001,1003]
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-6-assign-a-custom-security-attribute-with-a-boolean-value-to-a-user"></a>Пример 6. Назначение пользовательского атрибута безопасности с логическим значением пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с логическим значением.

- Набор атрибутов: `Engineering`
- Атрибут: `Certification`
- Тип данных атрибута: логический
- Значение атрибута: `true`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":true
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="update-custom-security-attribute-assignments"></a>Обновление пользовательских назначений атрибутов безопасности

### <a name="example-1-update-a-custom-security-attribute-assignment-with-an-integer-value-for-a-user"></a>Пример 1. Обновление пользовательского назначения атрибута безопасности с помощью целого значения для пользователя

В следующем примере показано, как обновить пользовательское назначение атрибута безопасности целочисленным значением для пользователя.

- Набор атрибутов: `Engineering`
- Атрибут: `NumVendors`
- Тип данных атрибута: Целое число
- Значение атрибута: `8`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":8
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-update-a-custom-security-attribute-assignment-with-a-boolean-value-for-a-user"></a>Пример 2. Обновление пользовательского назначения атрибута безопасности с помощью логического значения для пользователя

В следующем примере показано, как обновить пользовательское назначение атрибута безопасности на логическое значение для пользователя.

- Набор атрибутов: `Engineering`
- Атрибут: `Certification`
- Тип данных атрибута: логический
- Значение атрибута: `false`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":false
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remove-custom-security-attribute-assignments"></a>Удаление пользовательских назначений атрибутов безопасности

### <a name="example-1-remove-a-single-valued-custom-security-attribute-assignment-from-a-user"></a>Пример 1. Удаление одно значение настраиваемого назначения атрибутов безопасности от пользователя

В следующем примере показано, как удалить пользовательское назначение атрибута безопасности, которое поддерживает одно значение пользователя.

- Набор атрибутов: `Engineering`
- Атрибут: `ProjectDate`
- Значение атрибута: `null`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_singlevalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":null
        }
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-multi-valued-custom-security-attribute-assignment-from-a-user"></a>Пример 2. Удаление присваивания пользователю настраиваемых атрибутов безопасности с несколькими значениями

В следующем примере показано, как удалить пользовательское назначение атрибута безопасности, которое поддерживает несколько значений от пользователя.

- Набор атрибутов: `Engineering`
- Атрибут: `Project`
- Значение атрибута: `[]`

#### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_multivalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project":[]
        }
    }
}
```

#### <a name="response"></a>Ответ
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="next-steps"></a>Дальнейшие действия

- [Обзор настраиваемых атрибутов безопасности с помощью microsoft API Graph (предварительная версия)](/graph/api/resources/custom-security-attributes-overview)
- [Что такое настраиваемые атрибуты безопасности в Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)
