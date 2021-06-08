---
title: Обновление синхронизацииSchema
description: Обновление схемы синхронизации для данного задания или шаблона. Этот метод полностью заменяет текущую схему на схему, представленную в запросе. Чтобы обновить схему шаблона, необходимо вызвать объект приложения. Вы должны быть владельцем приложения.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bae3e92c82680dbf4f376e54bb5353ccb7851706
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786918"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="ac3df-106">Обновление синхронизацииSchema</span><span class="sxs-lookup"><span data-stu-id="ac3df-106">Update synchronizationSchema</span></span>

<span data-ttu-id="ac3df-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac3df-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac3df-108">Обновление схемы синхронизации для данного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="ac3df-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="ac3df-109">Этот метод полностью заменяет текущую схему на схему, представленную в запросе.</span><span class="sxs-lookup"><span data-stu-id="ac3df-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="ac3df-110">Чтобы обновить схему шаблона, необходимо вызвать объект приложения.</span><span class="sxs-lookup"><span data-stu-id="ac3df-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="ac3df-111">Вы должны быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="ac3df-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac3df-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3df-112">Permissions</span></span>
<span data-ttu-id="ac3df-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac3df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac3df-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3df-115">Permission type</span></span>                        | <span data-ttu-id="ac3df-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac3df-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac3df-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac3df-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="ac3df-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac3df-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ac3df-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac3df-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ac3df-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac3df-120">Not supported.</span></span>|
|<span data-ttu-id="ac3df-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="ac3df-121">Application</span></span>                            |<span data-ttu-id="ac3df-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac3df-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ac3df-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac3df-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="ac3df-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ac3df-124">Request headers</span></span>

| <span data-ttu-id="ac3df-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ac3df-125">Name</span></span>           | <span data-ttu-id="ac3df-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ac3df-126">Type</span></span>    | <span data-ttu-id="ac3df-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3df-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ac3df-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac3df-128">Authorization</span></span>  | <span data-ttu-id="ac3df-129">string</span><span class="sxs-lookup"><span data-stu-id="ac3df-129">string</span></span>  | <span data-ttu-id="ac3df-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac3df-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac3df-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac3df-132">Request body</span></span>

<span data-ttu-id="ac3df-133">В теле запроса поставляют объект [синхронизацииSchema](../resources/synchronization-synchronizationschema.md) для замены существующей схемы.</span><span class="sxs-lookup"><span data-stu-id="ac3df-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="ac3df-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac3df-134">Response</span></span>

<span data-ttu-id="ac3df-135">В случае успешной работы возвращается `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="ac3df-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="ac3df-136">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac3df-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac3df-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ac3df-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac3df-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac3df-138">Request</span></span>
<span data-ttu-id="ac3df-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac3df-139">The following is an example of a request.</span></span>

><span data-ttu-id="ac3df-140">**Примечание:** Показанный здесь объект запроса сокращается для читаемости.</span><span class="sxs-lookup"><span data-stu-id="ac3df-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="ac3df-141">Поставляем все свойства в реальном вызове.</span><span class="sxs-lookup"><span data-stu-id="ac3df-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac3df-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac3df-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac3df-143">C#</span><span class="sxs-lookup"><span data-stu-id="ac3df-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac3df-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac3df-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac3df-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac3df-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac3df-146">Java</span><span class="sxs-lookup"><span data-stu-id="ac3df-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac3df-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac3df-147">Response</span></span>
<span data-ttu-id="ac3df-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac3df-148">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response"
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


