---
title: 'ediscoveryReviewSet: addToReviewSet'
description: Начните процесс добавления коллекции из служб Microsoft 365 в набор для проверки.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8ae8a25bb90e647c4bd4795febf321a2a7208421
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946308"
---
# <a name="ediscoveryreviewset-addtoreviewset"></a>ediscoveryReviewSet: addToReviewSet
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Начните процесс добавления коллекции из служб Microsoft 365 в набор для проверки. После создания операции можно `Location` получить состояние операции, получив параметр из заголовков ответа. Расположение содержит URL-адрес, который возвращает операцию ["Добавить для проверки набора"](../resources/security-ediscoveryaddtoreviewsetoperation.md).


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
POST /ediscoveryExportOperation/reviewSet/addToReviewSet
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
POST https://graph.microsoft.com/beta/ediscoveryExportOperation/reviewSet/addToReviewSet
Content-Type: application/json

{
    "search": {
        "id": "7c165312-d8db-48b5-9129-1af50932df53"
    },
    "additionalDataOptions": "linkedFiles"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```