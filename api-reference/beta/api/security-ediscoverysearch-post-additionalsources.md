---
title: Создание источника данных
description: Создайте объект dataSource.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 625670c04c308ca1ca30ff0f9f9a2b2435211663
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946239"
---
# <a name="create-datasource"></a>Создание источника данных
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект dataSource.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [dataSource](../resources/security-datasource.md) в формате JSON.

При создании **источника данных** можно указать следующие свойства.

>**Примечание:** Требуется **либо адрес электронной** **почты** , либо сайт, а не оба. 

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|строка|SMTP-адрес почтового ящика. Чтобы получить адрес электронной почты группы, используйте группы [list или](../api/group-list.md) [Get](../api/group-get.md). Можно выполнить запрос по имени группы, используя `$filter`, например, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName`.|
|site|string|URL-адрес сайта; Например, `https://contoso.sharepoint.com/sites/HumanResources`. |


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает значение `201 Created`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources

{
    "@odata.type": "microsoft.graph.security.siteSource",
    "site": {
        "webUrl": "https://contoso.sharepoint.com/sites/SecretSite"
    }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.dataSource"
}
-->
``` http
HTTP/1.1 201 Created

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('15d80234-8320-4f10-96d0-d98d53ffdfc9')/sourceCollections('39b0bafd920e4360995c62e18a5e8a49')/additionalSources/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.siteSource",
    "displayName": "Secret Site",
    "createdDateTime": "2021-08-11T23:35:02.33986Z",
    "id": "42393244-3838-4636-3437-453030334136",
    "createdBy": {
        "user": {
            "id": "798d8d23-2087-4e03-912e-c0d9db5cb5d2",
            "displayName": "Edisco Admin",
            "userPrincipalname": "ediscoadmin@contoso.com"
        }
    }
}
```