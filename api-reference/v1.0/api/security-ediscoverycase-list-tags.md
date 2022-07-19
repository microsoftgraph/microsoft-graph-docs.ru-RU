---
title: Перечисление тегов
description: Получение списка объектов ediscoveryReviewTag из объекта дела eDiscovery.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e0de45515742fb2c32aedcf51a3e73623c45f5df
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839932"
---
# <a name="list-tags"></a>Перечисление тегов
Пространство имен: microsoft.graph.security

Получение списка объектов [eDiscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) и их свойств.

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик

В случае успешного `200 OK` выполнения этот метод возвращает код отклика и коллекцию объектов [microsoft.graph.security.ediscoveryreviewtag](../resources/security-ediscoveryreviewtag.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewtag_from_"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags",
    "@odata.count": 5,
    "value": [
        {
            "displayName": "My tag",
            "lastModifiedDateTime": "2022-05-23T19:41:01.7432683Z",
            "childSelectability": "Many",
            "id": "062de822f17a4a2e9b833aa3f6c37108",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "displayName": "Responsive",
            "description": "",
            "lastModifiedDateTime": "2022-05-23T19:41:24.4237284Z",
            "childSelectability": "One",
            "id": "d3d99dc704a74801b792b3e1e722aa0d",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "displayName": "Not responsive",
            "lastModifiedDateTime": "2022-05-23T19:41:31.3381716Z",
            "childSelectability": "One",
            "id": "ced26633616a434abd83762d49a25a6c",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "displayName": "Processing",
            "description": "Determine whether to outsource processing",
            "lastModifiedDateTime": "2022-05-23T19:46:03.8746996Z",
            "childSelectability": "Many",
            "id": "d8580989505c4fb3a25b845013697cf7",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "displayName": "External",
            "lastModifiedDateTime": "2022-05-23T19:46:10.5212362Z",
            "childSelectability": "One",
            "id": "d05c2ef9369d49c293b5a6a6d18a5fd9",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        }
    ]
}
```
