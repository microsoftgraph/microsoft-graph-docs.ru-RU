---
title: Обновление synchronizationSchema
description: Обновление схемы синхронизации для данного задания или шаблона. Этот метод полностью заменяет текущей схеме в запросе. Для обновления схемы шаблона, звонок на объект приложения. Необходимо быть владельцем приложения.
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525551"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="4ca51-106">Обновление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="4ca51-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca51-107">Обновление схемы синхронизации для данного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="4ca51-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="4ca51-108">Этот метод полностью заменяет текущей схеме в запросе.</span><span class="sxs-lookup"><span data-stu-id="4ca51-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="4ca51-109">Для обновления схемы шаблона, звонок на объект приложения.</span><span class="sxs-lookup"><span data-stu-id="4ca51-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="4ca51-110">Необходимо быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="4ca51-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ca51-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca51-111">Permissions</span></span>
<span data-ttu-id="4ca51-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca51-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca51-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca51-114">Permission type</span></span>                        | <span data-ttu-id="4ca51-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ca51-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ca51-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ca51-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="4ca51-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ca51-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4ca51-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ca51-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4ca51-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca51-119">Not supported.</span></span>|
|<span data-ttu-id="4ca51-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ca51-120">Application</span></span>                            |<span data-ttu-id="4ca51-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca51-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4ca51-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ca51-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="4ca51-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ca51-123">Request headers</span></span>

| <span data-ttu-id="4ca51-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4ca51-124">Name</span></span>           | <span data-ttu-id="4ca51-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4ca51-125">Type</span></span>    | <span data-ttu-id="4ca51-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca51-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4ca51-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ca51-127">Authorization</span></span>  | <span data-ttu-id="4ca51-128">string</span><span class="sxs-lookup"><span data-stu-id="4ca51-128">string</span></span>  | <span data-ttu-id="4ca51-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ca51-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ca51-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ca51-131">Request body</span></span>

<span data-ttu-id="4ca51-132">В тексте запроса предоставить объект [synchronizationSchema](../resources/synchronization-synchronizationschema.md) для замены существующей схемы с.</span><span class="sxs-lookup"><span data-stu-id="4ca51-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="4ca51-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ca51-133">Response</span></span>

<span data-ttu-id="4ca51-134">В случае успеха возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="4ca51-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="4ca51-135">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ca51-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca51-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4ca51-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4ca51-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ca51-137">Request</span></span>
<span data-ttu-id="4ca51-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ca51-138">The following is an example of a request.</span></span>

><span data-ttu-id="4ca51-139">**Примечание:** Объект запроса, показанный сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="4ca51-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="4ca51-140">Предоставить все свойства фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="4ca51-140">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

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

##### <a name="response"></a><span data-ttu-id="4ca51-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ca51-141">Response</span></span>
<span data-ttu-id="4ca51-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4ca51-142">The following is an example of a response.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
