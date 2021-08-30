---
title: Создание externalDomainName
description: Создание нового объекта externalDomainName.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1eb7e580fb5e2c469eaece2889a236b4cde02b6d
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697065"
---
# <a name="create-externaldomainname"></a>Создание externalDomainName
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте несколько доменов в конфигурацию SAML или WS-Fed, создав новый объект [externalDomainName](../resources/externaldomainname.md) и добавьте его в существующий [samlOrWsFedExternalDomainFedFedFedAinFederation.](../resources/samlorwsfedexternaldomainfederation.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Domain.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Domain.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать одной из следующих ролей Azure Active Directory [(Azure AD):](/azure/active-directory/roles/permissions-reference)

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса подарим JSON представление [объекта externalDomainName.](../resources/externaldomainname.md)

В следующей таблице показаны свойства, необходимые при создании [externalDomainName.](../resources/externaldomainname.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Доменное имя внешней организации, которое необходимо добавить в [samlOrOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md) Наследуется от [сущности](../resources/entity.md).|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект externalDomainName](../resources/externaldomainname.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_externaldomainname_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations/d5a56845-6845-d5a5-4568-a5d54568a5d5/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
Content-Type: application/json
Content-length: 60

{
    "@odata.type": "microsoft.graph.externalDomainName",
    "id": "contososuites.com"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalDomainName"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "contososuites.com"
}
```
