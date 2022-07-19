---
title: Удаление ediscoveryReviewSetQuery
description: Удаление объекта ediscoveryReviewSetQuery.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 233a2e403020550fe06d26d19ef6ef5ff18e3927
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838502"
---
# <a name="delete-ediscoveryreviewsetquery"></a>Удаление ediscoveryReviewSetQuery
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление объекта [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .

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
DELETE /security/cases/ediscoverycases/{eDiscoveryCaseId}}/reviewSets/{ediscoveryReviewSetId}/queries/{eDiscoveryReviewSetQueryId}
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
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_ediscoveryreviewsetquery"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/63ef0fd7-0db2-45eb-a9d7-7d75c8239873/queries/b7f4961d-59b1-444f-a4ec-57f2e5c2bf21
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

