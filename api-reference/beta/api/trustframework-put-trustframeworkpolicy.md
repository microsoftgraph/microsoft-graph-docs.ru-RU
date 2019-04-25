---
title: Обновление Трустфрамеворкполици
description: 'Эта операция обновляет существующий объект Трустфрамеворкполици или, если таковой не существует, создает его. '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de2327489d6606c40fe55934d333f2fd2f9c0b44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536980"
---
# <a name="update-or-create-trustframeworkpolicy"></a>Обновление или создание Трустфрамеворкполици

>**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновите существующий [трустфрамеворкполици](../resources/trustframeworkpolicy.md) или создайте его, если он не существует.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Policy. ReadWrite. Трустфрамеворк, Policy. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|Не поддерживается.|

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
|Content-Type|Application/XML. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) . 

>**Note:** тип контента должен быть `application/xml`.

## <a name="response"></a>Ответ

Ответ будет одним из следующих вариантов:
- Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) существует, успешный запрос возвращает код `200 OK` отклика.
- Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) не существует, успешный запрос возвращает код `201 Created` отклика.
- В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="example"></a>Пример

В следующем примере показано, как обновить объект **трустфрамеворкполици**.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type:application/xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
