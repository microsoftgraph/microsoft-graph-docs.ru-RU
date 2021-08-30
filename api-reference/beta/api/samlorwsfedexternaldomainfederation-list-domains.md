---
title: Список доменов
description: Получите список всех объектов externalDomainName для samlOrWsFedExternalDomainFederation.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d6fbb65435107a1ef932ab4be3b330f87e0b80d1
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697073"
---
# <a name="list-domains"></a>Список доменов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список всех [объектов externalDomainName](../resources/externaldomainname.md) для [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.Read.All, Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.Read.All, Domain.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать одной из следующих ролей Azure Active Directory [(Azure AD):](/azure/active-directory/roles/permissions-reference)

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation/{samlOrWsFedExternalDomainFederation ID}/domains
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов externalDomainName](../resources/externaldomainname.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list_externaldomainname"
}
-->

``` http
GET https://graph.microsoft.com/beta/directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation/f1e11a04-0244-4592-99df-b01cfaadce15/domains
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalDomainName)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation('f1e11a04-0244-4592-99df-b01cfaadce15')/domains",
    "value": [
        {
            "id": "fabrikam.com"
        },
        {
            "id": "contoso.com"
        }
    ]
}
```
