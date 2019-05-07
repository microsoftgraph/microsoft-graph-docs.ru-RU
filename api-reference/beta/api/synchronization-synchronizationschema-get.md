---
title: Получение Синчронизатионсчема
description: Получение схемы для данного задания или шаблона синхронизации.
localization_priority: Normal
ms.openlocfilehash: 3b834d955a79c45ef5ae1e43ec9ca0f1fd18cedd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637964"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="3c6d3-103">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="3c6d3-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c6d3-104">Получение схемы для данного задания или шаблона синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c6d3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c6d3-105">Permissions</span></span>
<span data-ttu-id="3c6d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c6d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c6d3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c6d3-108">Permission type</span></span>                        | <span data-ttu-id="3c6d3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c6d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c6d3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c6d3-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="3c6d3-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c6d3-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3c6d3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c6d3-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3c6d3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-113">Not supported.</span></span> |
|<span data-ttu-id="3c6d3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c6d3-114">Application</span></span>                            |<span data-ttu-id="3c6d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3c6d3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c6d3-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="3c6d3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c6d3-117">Request headers</span></span>

| <span data-ttu-id="3c6d3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3c6d3-118">Name</span></span>           | <span data-ttu-id="3c6d3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3c6d3-119">Type</span></span>    | <span data-ttu-id="3c6d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3c6d3-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3c6d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c6d3-121">Authorization</span></span>  | <span data-ttu-id="3c6d3-122">string</span><span class="sxs-lookup"><span data-stu-id="3c6d3-122">string</span></span>  | <span data-ttu-id="3c6d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c6d3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c6d3-125">Request body</span></span>

<span data-ttu-id="3c6d3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c6d3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c6d3-127">Response</span></span>

<span data-ttu-id="3c6d3-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c6d3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3c6d3-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c6d3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c6d3-130">Request</span></span>
<span data-ttu-id="3c6d3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="3c6d3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c6d3-132">Response</span></span>
<span data-ttu-id="3c6d3-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-133">The following is an example of a response.</span></span>

><span data-ttu-id="3c6d3-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c6d3-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c6d3-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c6d3-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="3c6d3-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c6d3-137">Языках</span><span class="sxs-lookup"><span data-stu-id="3c6d3-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c6d3-138">Язык</span><span class="sxs-lookup"><span data-stu-id="3c6d3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
