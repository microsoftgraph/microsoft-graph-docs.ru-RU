---
title: Назначение, обновление или удаление настраиваемой атрибуты безопасности с помощью API microsoft Graph (Preview)
description: Узнайте, как назначать, обновлять или удалять настраиваемые атрибуты безопасности для пользователей и приложений (директоров служб) с помощью API microsoft Graph.
author: rolyon
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: directory-management
ms.openlocfilehash: fa046c1e55055ed1d8c00fdda67ea8be71c5d804
ms.sourcegitcommit: 709d2e3069765c2e570ac1128847c165ab233aa8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2022
ms.locfileid: "62184005"
---
# <a name="assign-update-or-remove-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>Назначение, обновление или удаление настраиваемой атрибуты безопасности с помощью API microsoft Graph (Preview)

> [!IMPORTANT]
> Функция пользовательских атрибутов безопасности в настоящее время находится в режиме Предварительного просмотра. Дополнительные термины использования для [Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) для юридических терминов, применимых к функциям Azure, которые находятся в бета-версии, предварительной версии или еще не выпущены в общую доступность.

[Настраиваемые](/azure/active-directory/fundamentals/custom-security-attributes-overview) атрибуты безопасности в Azure Active Directory (Azure AD) — это бизнес-атрибуты (пары значений ключей), которые можно определить и назначить объектам Azure AD.

В этой статье приводится пример назначения, обновления или удаления различных типов настраиваемого атрибута безопасности для пользователей и приложений (директоров служб). Настраиваемые атрибуты безопасности могут быть назначены или обновлены только с помощью операции в запросе `PATCH` [пользователя update](/graph/api/user-update?view=graph-rest-beta&preserve-view=true) или [update servicePrincipal.](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)

## <a name="permissions"></a>Разрешения

Чтобы управлять настраиваемой атрибутами безопасности, основной вызов должен быть назначен следующей роли Azure AD. По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

- [Администратор назначения атрибутов](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

Кроме того, директору по вызову должны быть предоставлены следующие разрешения.

- [CustomSecAttributeAssignment.ReadWrite.All](permissions-reference.md#custom-security-attributes-permissions)
- [User.Read.All](permissions-reference.md#user-permissions)

Разрешения на чтение, назначение, обновление или удаление атрибутов для приложения выданы *CustomSecAttributeAssignment.ReadWrite.All*. Разрешения на чтение объекта ресурса, например пользователей, выданы отдельно с помощью разрешений объектов ресурсов, таких как *User.Read.All.*

## <a name="assign-custom-security-attributes"></a>Назначение настраиваемой атрибуты безопасности

### <a name="example-1-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>Пример 1. Назначение пользовательского атрибута безопасности со значением строки пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности со значением строки.

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

### <a name="example-3-assign-a-custom-security-attribute-with-a-multi-string-value-to-a-user"></a>Пример 3. Назначить пользователю настраиваемый атрибут безопасности с многострунным значением

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с многострунным значением.

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

### <a name="example-4-assign-a-custom-security-attribute-with-an-integer-value-to-a-user"></a>Пример 4. Назначить пользователю настраиваемый атрибут безопасности со значением integer

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности со значением integer.

- Набор атрибутов: `Engineering`
- Атрибут: `NumVendors`
- Тип данных атрибута: Integer
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

### <a name="example-5-assign-a-custom-security-attribute-with-a-multi-integer-value-to-a-user"></a>Пример 5. Назначить пользователю настраиваемый атрибут безопасности с многоуровневым значением

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности с многоуровневым значением.

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

### <a name="example-6-assign-a-custom-security-attribute-with-a-boolean-value-to-a-user"></a>Пример 6. Назначение пользовательского атрибута безопасности со значением Boolean пользователю

В следующем примере показано, как назначить пользователю настраиваемый атрибут безопасности со значением Boolean.

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

### <a name="example-1-update-a-custom-security-attribute-assignment-with-an-integer-value-for-a-user"></a>Пример 1. Обновление настраиваемой назначения атрибута безопасности с помощью значения integer для пользователя

В следующем примере показано, как обновить настраиваемую назначение атрибута безопасности с помощью значения integer для пользователя.

- Набор атрибутов: `Engineering`
- Атрибут: `NumVendors`
- Тип данных атрибута: Integer
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


### <a name="example-2-update-a-custom-security-attribute-assignment-with-a-boolean-value-for-a-user"></a>Пример 2. Обновление настраиваемой назначения атрибута безопасности со значением Boolean для пользователя

В следующем примере показано, как обновить пользовательское назначение атрибута безопасности со значением Boolean для пользователя.

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

## <a name="remove-custom-security-attribute-assignments"></a>Удаление настраиваемой атрибутики безопасности

### <a name="example-1-remove-a-single-valued-custom-security-attribute-assignment-from-a-user"></a>Пример 1. Удалите одно значение настраиваемого назначения атрибута безопасности у пользователя

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

### <a name="example-2-remove-a-multi-valued-custom-security-attribute-assignment-from-a-user"></a>Пример 2. Удаление у пользователя нескольких значений настраиваемого атрибута безопасности

В следующем примере показано, как удалить пользовательское назначение атрибута безопасности, которое поддерживает несколько значений у пользователя.

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

- [Обзор пользовательских атрибутов безопасности с помощью API Graph Microsoft](/graph/api/resources/custom-security-attributes-overview)
- [Что такое настраиваемые атрибуты безопасности в Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)
- [Обновление пользователя](/graph/api/user-update?view=graph-rest-beta&preserve-view=true)
- [Обновить servicePrincipal](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)
