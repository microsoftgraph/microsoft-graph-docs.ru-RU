---
title: Обновление Синчронизатионсчема
description: Обновление схемы синхронизации для определенного задания или шаблона. Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе. Чтобы обновить схему шаблона, сделайте вызов для объекта Application. Вы должны быть владельцем приложения.
localization_priority: Normal
ms.openlocfilehash: 0990c1218d93b75e93b20271fc929621ab7e83e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458187"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="80990-106">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="80990-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80990-107">Обновление схемы синхронизации для определенного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="80990-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="80990-108">Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе.</span><span class="sxs-lookup"><span data-stu-id="80990-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="80990-109">Чтобы обновить схему шаблона, сделайте вызов для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="80990-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="80990-110">Вы должны быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="80990-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="80990-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80990-111">Permissions</span></span>
<span data-ttu-id="80990-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80990-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80990-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80990-114">Permission type</span></span>                        | <span data-ttu-id="80990-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80990-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="80990-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80990-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="80990-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80990-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="80990-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80990-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="80990-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80990-119">Not supported.</span></span>|
|<span data-ttu-id="80990-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80990-120">Application</span></span>                            |<span data-ttu-id="80990-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80990-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="80990-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80990-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="80990-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80990-123">Request headers</span></span>

| <span data-ttu-id="80990-124">Имя</span><span class="sxs-lookup"><span data-stu-id="80990-124">Name</span></span>           | <span data-ttu-id="80990-125">Тип</span><span class="sxs-lookup"><span data-stu-id="80990-125">Type</span></span>    | <span data-ttu-id="80990-126">Описание</span><span class="sxs-lookup"><span data-stu-id="80990-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="80990-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="80990-127">Authorization</span></span>  | <span data-ttu-id="80990-128">string</span><span class="sxs-lookup"><span data-stu-id="80990-128">string</span></span>  | <span data-ttu-id="80990-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80990-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80990-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80990-131">Request body</span></span>

<span data-ttu-id="80990-132">В теле запроса добавьте объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) для замены существующей схемы.</span><span class="sxs-lookup"><span data-stu-id="80990-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="80990-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="80990-133">Response</span></span>

<span data-ttu-id="80990-134">В случае успеха возвращает код `204 No Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="80990-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="80990-135">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="80990-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80990-136">Пример</span><span class="sxs-lookup"><span data-stu-id="80990-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80990-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="80990-137">Request</span></span>
<span data-ttu-id="80990-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80990-138">The following is an example of a request.</span></span>

><span data-ttu-id="80990-139">**Примечание:** Объект Request, показанный здесь, сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="80990-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="80990-140">Предоставьте все свойства в фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="80990-140">Supply all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80990-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="80990-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="80990-142">C#</span><span class="sxs-lookup"><span data-stu-id="80990-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80990-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="80990-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80990-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="80990-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80990-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="80990-145">Response</span></span>
<span data-ttu-id="80990-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80990-146">The following is an example of a response.</span></span>
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
