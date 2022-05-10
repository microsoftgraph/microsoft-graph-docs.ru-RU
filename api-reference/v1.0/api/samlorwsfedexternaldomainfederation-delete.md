---
title: Удаление samlOrWsFedExternalDomainFederation
description: Удаление объекта samlOrWsFedExternalDomainFederation.
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e2134d32854967e6ce07effbcd1c62af128a4a4a
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296663"
---
# <a name="delete-samlorwsfedexternaldomainfederation"></a>Удаление samlOrWsFedExternalDomainFederation
Пространство имен: microsoft.graph

Удаление объекта [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.ReadWrite.All|

Учетная запись рабочей или учебной учетной записи должна принадлежать одной из следующих Azure Active Directory [(Azure AD) ролей](/azure/active-directory/roles/permissions-reference):

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "delete_samlorwsfedexternaldomainfederation"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/directory/federationConfigurations/96db02e2-80c1-5555-bc3a-de92ffb8c5be
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
