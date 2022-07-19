---
title: Get ediscoveryCustodian
description: Чтение свойств и связей объекта ediscoveryCustodian.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6d60dba2215bc66c4c42938755ce6331d4746354
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839902"
---
# <a name="get-ediscoverycustodian"></a>Get ediscoveryCustodian
Пространство имен: microsoft.graph.security



Чтение свойств и связей объекта [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{ediscoveryCustodianId}
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}/custodian
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и объект [microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycustodian"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryCustodian"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians/$entity",
    "status": "active",
    "holdStatus": "applied",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2022-05-23T02:35:42.9272828Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "0053a61a3b6c42738f7606791716a22a",
    "displayName": "Alex Wilber",
    "email": "AlexW@M365x809305.OnMicrosoft.com",
    "acknowledgedDateTime": "0001-01-01T00:00:00Z"
}
```
