---
title: Обновление trustFrameworkPolicy
description: 'Эта операция обновляет существующий объект trustFrameworkPolicy, или если его не существует, она создает его. '
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b20d580ac7f5e273e66b1fdd152e7e607907b4df91276e8e76a5da697f9085c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54166017"
---
# <a name="update-or-create-trustframeworkpolicy"></a>Обновление или создание trustFrameworkPolicy

Пространство имен: microsoft.graph

>**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обнови [существующее довериеFrameworkPolicy](../resources/trustframeworkpolicy.md) или создайте его, если оно не существует.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.TrustFramework|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Policy.ReadWrite.TrustFramework|

Рабочая или учебная учетная запись должна быть глобальным администратором клиента.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/xml. Обязательно.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи XML-представление [объекта trustFrameworkPolicy.](../resources/trustframeworkpolicy.md) 

>**Примечание:** тип контента должен быть `application/xml` .

## <a name="response"></a>Отклик

Ответ будет одним из следующих:
- Если существует [trustFrameworkPolicy,](../resources/trustframeworkpolicy.md) успешный запрос возвращает `200 OK` код ответа.
- Если [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) не существует, успешный запрос возвращает `201 Created` код ответа.
- В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="example"></a>Пример

В следующем примере **обновляется trustFrameworkPolicy.**

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


