---
title: 'ediscoveryReviewSetQuery: applyTags'
description: Применение тегов к файлам в наборе проверки обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6e55eb34b162628d5dfd48536e3867b93ba722d3
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839542"
---
# <a name="ediscoveryreviewsetquery-applytags"></a>ediscoveryReviewSetQuery: applyTags
Пространство имен: microsoft.graph.security



Применение тегов к файлам в наборе проверки [обнаружения электронных данных](../resources/security-ediscoveryreviewset.md). Дополнительные сведения см [. в разделе "Пометка документов в наборе для проверки в службе обнаружения электронных данных"](/microsoft-365/compliance/tagging-documents).

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}/applyTags
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
|tagsToAdd|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Теги, удаляемые из файлов в запросе набора проверки.|
|tagsToRemove|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Теги для удаления добавляют файлы в запросе набора проверки.|



## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetquerythis.applytags"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/63ef0fd7-0db2-45eb-a9d7-7d75c8239873/queries/5f426fdc-f027-40db-b7cc-453cf06dc996/applyTags
Content-Type: application/json

{
    "tagsToAdd": [
        {"id": "d3d99dc704a74801b792b3e1e722aa0d"}
    ]
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
