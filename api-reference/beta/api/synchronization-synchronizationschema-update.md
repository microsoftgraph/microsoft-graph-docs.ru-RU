---
title: Обновление Синчронизатионсчема
description: Обновление схемы синхронизации для определенного задания или шаблона. Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе. Чтобы обновить схему шаблона, сделайте вызов для объекта Application. Вы должны быть владельцем приложения.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8211b5fc15e6648fea9ba1b4b44c28a93eb5e0f5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452906"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="92ea8-106">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="92ea8-106">Update synchronizationSchema</span></span>

<span data-ttu-id="92ea8-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92ea8-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ea8-108">Обновление схемы синхронизации для определенного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="92ea8-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="92ea8-109">Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе.</span><span class="sxs-lookup"><span data-stu-id="92ea8-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="92ea8-110">Чтобы обновить схему шаблона, сделайте вызов для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="92ea8-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="92ea8-111">Вы должны быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="92ea8-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="92ea8-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92ea8-112">Permissions</span></span>
<span data-ttu-id="92ea8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ea8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ea8-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92ea8-115">Permission type</span></span>                        | <span data-ttu-id="92ea8-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92ea8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ea8-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92ea8-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="92ea8-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ea8-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="92ea8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92ea8-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="92ea8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ea8-120">Not supported.</span></span>|
|<span data-ttu-id="92ea8-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92ea8-121">Application</span></span>                            |<span data-ttu-id="92ea8-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ea8-122">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="92ea8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92ea8-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="92ea8-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92ea8-124">Request headers</span></span>

| <span data-ttu-id="92ea8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="92ea8-125">Name</span></span>           | <span data-ttu-id="92ea8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="92ea8-126">Type</span></span>    | <span data-ttu-id="92ea8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="92ea8-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="92ea8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ea8-128">Authorization</span></span>  | <span data-ttu-id="92ea8-129">string</span><span class="sxs-lookup"><span data-stu-id="92ea8-129">string</span></span>  | <span data-ttu-id="92ea8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92ea8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92ea8-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92ea8-132">Request body</span></span>

<span data-ttu-id="92ea8-133">В теле запроса добавьте объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) для замены существующей схемы.</span><span class="sxs-lookup"><span data-stu-id="92ea8-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="92ea8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ea8-134">Response</span></span>

<span data-ttu-id="92ea8-135">В случае успеха возвращает код `204 No Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="92ea8-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="92ea8-136">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="92ea8-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ea8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="92ea8-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92ea8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="92ea8-138">Request</span></span>
<span data-ttu-id="92ea8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92ea8-139">The following is an example of a request.</span></span>

><span data-ttu-id="92ea8-140">**Примечание:** Объект Request, показанный здесь, сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92ea8-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="92ea8-141">Предоставьте все свойства в фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="92ea8-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="92ea8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="92ea8-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92ea8-143">C#</span><span class="sxs-lookup"><span data-stu-id="92ea8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92ea8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92ea8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92ea8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92ea8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92ea8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ea8-146">Response</span></span>
<span data-ttu-id="92ea8-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92ea8-147">The following is an example of a response.</span></span>
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
