---
title: Создание noncustodialDataSource
description: Создайте новый объект noncustodialDataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 87817dfed8b4ba12c98661e847aa7e44302a7771
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080860"
---
# <a name="create-noncustodialdatasource"></a>Создание noncustodialDataSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса подарят представление JSON объекта [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

В следующей таблице показаны свойства, необходимые при создании [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|applyHoldToSource|Boolean|Указывает, применяется ли удержание к источнику данных без хранения (например, к почтовому ящику или сайту).|
|datasource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Либо userSource, либо siteSource.  Для userSource используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.  Для источника сайта используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.siteSource", "site@odata.bind": "siteId" }, где siteId можно извлечь из URL-адреса сайта, например, запрос Microsoft Graph будет `https://contoso.sharepoint.com/sites/HumanResources` `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` . ID — это первый GUID, указанный в поле ID.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json
Content-length: 206

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```
