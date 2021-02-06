---
title: Обновление synchronizationSchema
description: Обновление схемы синхронизации для заданного задания или шаблона. Этот метод полностью заменяет текущую схему схемой, предоставленной в запросе. Чтобы обновить схему шаблона, вызовите объект приложения. Вы должны быть владельцем приложения.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 9c6ce22d5b6811f777667af53d4b6df82a4b372b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136355"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="9c6a5-106">Обновление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="9c6a5-106">Update synchronizationSchema</span></span>

<span data-ttu-id="9c6a5-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c6a5-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c6a5-108">Обновление схемы синхронизации для заданного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="9c6a5-109">Этот метод полностью заменяет текущую схему схемой, предоставленной в запросе.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="9c6a5-110">Чтобы обновить схему шаблона, вызовите объект приложения.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="9c6a5-111">Вы должны быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c6a5-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c6a5-112">Permissions</span></span>
<span data-ttu-id="9c6a5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c6a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c6a5-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c6a5-115">Permission type</span></span>                        | <span data-ttu-id="9c6a5-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c6a5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c6a5-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c6a5-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="9c6a5-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c6a5-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9c6a5-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c6a5-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9c6a5-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-120">Not supported.</span></span>|
|<span data-ttu-id="9c6a5-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c6a5-121">Application</span></span>                            |<span data-ttu-id="9c6a5-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-122">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="9c6a5-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c6a5-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="9c6a5-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c6a5-124">Request headers</span></span>

| <span data-ttu-id="9c6a5-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9c6a5-125">Name</span></span>           | <span data-ttu-id="9c6a5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9c6a5-126">Type</span></span>    | <span data-ttu-id="9c6a5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9c6a5-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9c6a5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c6a5-128">Authorization</span></span>  | <span data-ttu-id="9c6a5-129">string</span><span class="sxs-lookup"><span data-stu-id="9c6a5-129">string</span></span>  | <span data-ttu-id="9c6a5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c6a5-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c6a5-132">Request body</span></span>

<span data-ttu-id="9c6a5-133">В теле запроса укажи объект [synchronizationSchema](../resources/synchronization-synchronizationschema.md) для замены существующей схемы.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="9c6a5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c6a5-134">Response</span></span>

<span data-ttu-id="9c6a5-135">В случае успеха возвращает код `204 No Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="9c6a5-136">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c6a5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9c6a5-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9c6a5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c6a5-138">Request</span></span>
<span data-ttu-id="9c6a5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-139">The following is an example of a request.</span></span>

><span data-ttu-id="9c6a5-140">**Примечание.** Показанный здесь объект запроса сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="9c6a5-141">Укавите все свойства в реальном вызове.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c6a5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c6a5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
Content-type: application/json

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
                },
            ]
        },
        {
            "name": "Salesforce",
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
                    ]
                },
            ]
        },
    ]
}

```
# <a name="c"></a>[<span data-ttu-id="9c6a5-143">C#</span><span class="sxs-lookup"><span data-stu-id="9c6a5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c6a5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c6a5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c6a5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c6a5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c6a5-146">Java</span><span class="sxs-lookup"><span data-stu-id="9c6a5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9c6a5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c6a5-147">Response</span></span>
<span data-ttu-id="9c6a5-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c6a5-148">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


