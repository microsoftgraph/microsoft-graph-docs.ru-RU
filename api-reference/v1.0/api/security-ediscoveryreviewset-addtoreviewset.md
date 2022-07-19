---
title: 'ediscoveryReviewSet: addToReviewSet'
description: Начните процесс добавления коллекции из служб Microsoft 365 в набор для проверки.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 30d4093704cc683f97f9dfb4334b193341bf4fad
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839812"
---
# <a name="ediscoveryreviewset-addtoreviewset"></a>ediscoveryReviewSet: addToReviewSet
Пространство имен: microsoft.graph.security



Начните процесс добавления коллекции из служб Microsoft 365 в [набор для проверки](../resources/security-ediscoveryreviewset.md). После создания операции можно `Location` получить состояние операции, получив параметр из заголовков ответа. Расположение содержит URL-адрес, который возвращает операцию ["Добавить для проверки набора"](../resources/security-ediscoveryaddtoreviewsetoperation.md).


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
POST /security/cases/ediscoverycases/{eDiscoveryCaseId}/reviewSets/{eDiscoveryReviewSetId}/addToReviewSet
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Идентификатор поиска eDiscovery, который вы хотите добавить в набор для проверки.|
|additionalDataOptions|additionalDataOptions|Параметры для добавления элементов в reviewSet.|

### <a name="additionaldataoptions-values"></a>Значения additionalDataOptions
|Имя|Описание|
|:---|:---|
|allVersions|включают все версии документа SharePoint, соответствующие запросу исходной коллекции. Внимание! Версии SharePoint могут значительно увеличить объем элементов |
|linkedFiles|включите связанные файлы, к которым был предоставлен общий доступ в сообщениях Outlook, teams или Yammer, путем вложения ссылки на файл.|

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.addtoreviewset"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/63ef0fd7-0db2-45eb-a9d7-7d75c8239873/addToReviewSet
Content-Type: application/json

{
    "search": {
        "id": "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7"
    },
    "additionalDataOptions": "linkedFiles"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```