---
title: Создание educationSubmissionResource
description: Добавьте ресурс в список ресурсов отправки.
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6752e07f379e444b5f4fc80fcb77e7204886113a
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936007"
---
# <a name="create-educationsubmissionresource"></a>Создание educationSubmissionResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте ресурс в список ресурсов отправки.

Выполнить эту операцию может только студент, назначенный для отправки.

Операция не будет успешной, если флаг **allowStudentsToAddResources** не `true` установлен. 

Чтобы создать новый ресурс на основе файлов, загрузите файл в папку ресурсов, связанную с отправкой. Если файл не существует или не находится в этой папке, запрос POST не будет работать.

> [!IMPORTANT] 
> Перед отправкой ресурса назначения необходимо [](../api/educationassignment-setupresourcesfolder.md) настроить папку ресурсов для [educationAssignment](../resources/educationassignment.md) для отправки файлов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
|Для приложений | Не поддерживается. | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{class-id}/assignments/{assignment-id}/submissions/{submission-id}/resources
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON ресурса. Следующие поддерживаемые типы:

- [educationExcelResource](../resources/educationexcelresource.md)
- [educationFileResource](../resources/educationfileresource.md)
- [educationLinkResource](../resources/educationlinkresource.md)
- [educationPowerPointResource](../resources/educationpowerpointresource.md)
- [educationWordResource](../resources/educationwordresource.md) 
- [educationMediaResource](../resources/educationmediaresource.md).

>**Примечание:** [EducationExternalResource](../resources/educationexternalresource.md) — это только ресурс, с помощью него нельзя опубликовать отправку.

Не `assignmentResourceUrl` требуется в тексте запроса, это свойство только для чтения.

## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код ответа и объект в соответствии с типом ресурса `201 Created` в тексте ответа.

## <a name="examples"></a>Примеры
### <a name="example-1-create-an-educationwordresource"></a>Пример 1. Создание educationWordResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationwordresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b/submissions/4af73d2b-6b9c-493f-0688-979087bed39b/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "microsoft.graph.educationWordResource",
        "displayName": "Report.docx",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationwordresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationwordresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationwordresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationwordresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationWordResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('f4a941ff-9da6-4707-ba5b-0eae93cad0b4')/assignments('3c77de7f-539b-49e1-9c96-1274f2f0ee3b')/submissions('4af73d2b-6b9c-493f-0688-979087bed39b')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "d835503f-fd00-4840-b69c-7230d10e18b8",
    "resource": {
        "@odata.type": "#microsoft.graph.educationWordResource",
        "displayName": "Report.docx",
        "createdDateTime": "2021-08-04T00:23:08.6269586Z",
        "lastModifiedDateTime": "2021-08-04T00:23:08.6269586Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-2-create-an-educationlinkresource"></a>Пример 2. Создание образованияLinkResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationlinkresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources
Content-type: application/json

{
    "resource": {
        "displayName": "Wikipedia",
        "link": "https://en.wikipedia.org/wiki/Main_Page",
        "@odata.type": "#microsoft.graph.educationLinkResource"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationlinkresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationlinkresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationlinkresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationlinkresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationLinkResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions('da443246-384d-673b-32db-bdba9d7f2b51')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "88b441b0-cb05-45ab-a0f0-139f978e0993",
    "resource": {
        "@odata.type": "#microsoft.graph.educationLinkResource",
        "displayName": "Wikipedia",
        "createdDateTime": "2021-09-13T19:20:46.0648354Z",
        "lastModifiedDateTime": "2021-09-13T19:20:46.0648354Z",
        "link": "https://en.wikipedia.org/wiki/Main_Page",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-3-create-an-educationfileresource"></a>Пример 3. Создание образованияFileResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationfileresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources
Content-type: application/json

{
    "resource": {
        "displayName": "_FTP_EDC-61424749-250820211136.pdf",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3",
        "@odata.type": "#microsoft.graph.educationFileResource"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationfileresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationfileresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationfileresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationfileresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions('da443246-384d-673b-32db-bdba9d7f2b51')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "33cf3eb2-8a35-4f76-8f16-b2abc112d44f",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "_FTP_EDC-61424749-250820211136.pdf",
        "createdDateTime": "2021-09-13T19:23:04.5049139Z",
        "lastModifiedDateTime": "2021-09-13T19:23:04.5049139Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-4-create-an-educationexcelresource"></a>Пример 4. Создание образованияExcelResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationexcelresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "#microsoft.graph.educationExcelResource",
        "displayName": "userAgeGroup QueryParameter Test.xlsx",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationexcelresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationexcelresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationexcelresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationexcelresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationExcelResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions('da443246-384d-673b-32db-bdba9d7f2b51')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "c36626ba-9864-4f3a-8d6f-7104f62df605",
    "resource": {
        "@odata.type": "#microsoft.graph.educationExcelResource",
        "displayName": "userAgeGroup QueryParameter Test.xlsx",
        "createdDateTime": "2021-09-13T19:23:58.3925618Z",
        "lastModifiedDateTime": "2021-09-13T19:23:58.3925618Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-5-create-an-educationpowerpointresource"></a>Пример 5. Создание образованияPowerPointResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationpowerpointresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "#microsoft.graph.educationPowerPointResource",
        "displayName": "state diagram.pptx",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationpowerpointresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationpowerpointresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationpowerpointresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationpowerpointresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPowerPointResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions('da443246-384d-673b-32db-bdba9d7f2b51')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "e19bd829-17ee-4483-88d0-f62b406f367c",
    "resource": {
        "@odata.type": "#microsoft.graph.educationPowerPointResource",
        "displayName": "state diagram.pptx",
        "createdDateTime": "2021-09-13T19:24:38.4706263Z",
        "lastModifiedDateTime": "2021-09-13T19:24:38.4706263Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-6-create-an-educationmediaresource"></a>Пример 6. Создание educationMediaResource
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","da443246-384d-673b-32db-bdba9d7f2b51"], 
  "name": "create_educationmediaresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources
Content-type: application/json

{
    "resource": {
        "displayName": "category.jpg",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG",
        "@odata.type": "#microsoft.graph.educationMediaResource"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationmediaresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationmediaresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationmediaresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationmediaresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationMediaResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions('da443246-384d-673b-32db-bdba9d7f2b51')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "31f2c67a-6df1-4a7f-b4c5-311fe15c873a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationMediaResource",
        "displayName": "category.jpg",
        "createdDateTime": "2021-09-16T19:07:59.4982929Z",
        "lastModifiedDateTime": "2021-09-16T19:07:59.4982929Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

## <a name="see-also"></a>См. также

* [Состояния, переходы и ограничения для назначений и представлений](/graph/assignments-submissions-states-transition)
* [Upload для назначений и представлений об образовании](/graph/education-upload-resource-overview)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


