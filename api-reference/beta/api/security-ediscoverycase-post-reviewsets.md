---
title: Создание объекта ediscoveryReviewSet
description: Создайте объект ediscoveryReviewSet.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8fa0afe57fe0f62e7f3713de92e1e8b2864dadff
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946468"
---
# <a name="create-ediscoveryreviewset"></a>Создание объекта ediscoveryReviewSet
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) в формате JSON.

При создании **ediscoveryReviewSet** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя набора для проверки. Обязательный.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и [объект ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/reviewSets
Content-Type: application/json

{
    "displayName": "My review set 2"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/reviewSets/$entity",
    "displayName": "My review set 2",
    "id": "887306f5-1eb4-4409-b18c-ba47f4e3fa9b",
    "createdDateTime": "2022-05-23T16:33:13.5126494Z",
    "createdBy": {
        "application": null,
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": null,
            "userPrincipalName": "c25c3914-f9f7-43ee-9cba-a25377e0cec6"
        }
    }
}
```

