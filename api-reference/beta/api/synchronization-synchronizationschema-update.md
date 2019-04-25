---
title: Обновление Синчронизатионсчема
description: Обновление схемы синхронизации для определенного задания или шаблона. Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе. Чтобы обновить схему шаблона, сделайте вызов для объекта Application. Вы должны быть владельцем приложения.
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536959"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="bc6a7-106">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="bc6a7-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc6a7-107">Обновление схемы синхронизации для определенного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="bc6a7-108">Этот метод полностью заменяет текущую схему на ту, которая была указана в запросе.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="bc6a7-109">Чтобы обновить схему шаблона, сделайте вызов для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="bc6a7-110">Вы должны быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc6a7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc6a7-111">Permissions</span></span>
<span data-ttu-id="bc6a7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc6a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc6a7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc6a7-114">Permission type</span></span>                        | <span data-ttu-id="bc6a7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc6a7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc6a7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc6a7-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="bc6a7-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6a7-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bc6a7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc6a7-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bc6a7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-119">Not supported.</span></span>|
|<span data-ttu-id="bc6a7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc6a7-120">Application</span></span>                            |<span data-ttu-id="bc6a7-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="bc6a7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc6a7-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="bc6a7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc6a7-123">Request headers</span></span>

| <span data-ttu-id="bc6a7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="bc6a7-124">Name</span></span>           | <span data-ttu-id="bc6a7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="bc6a7-125">Type</span></span>    | <span data-ttu-id="bc6a7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bc6a7-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bc6a7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc6a7-127">Authorization</span></span>  | <span data-ttu-id="bc6a7-128">string</span><span class="sxs-lookup"><span data-stu-id="bc6a7-128">string</span></span>  | <span data-ttu-id="bc6a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc6a7-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc6a7-131">Request body</span></span>

<span data-ttu-id="bc6a7-132">В теле запроса добавьте объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) для замены существующей схемы.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="bc6a7-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc6a7-133">Response</span></span>

<span data-ttu-id="bc6a7-134">В случае успеха возвращает код `204 No Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="bc6a7-135">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc6a7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="bc6a7-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc6a7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc6a7-137">Request</span></span>
<span data-ttu-id="bc6a7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-138">The following is an example of a request.</span></span>

><span data-ttu-id="bc6a7-139">**Примечание:** Объект Request, показанный здесь, сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="bc6a7-140">Предоставьте все свойства в фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-140">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bc6a7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc6a7-141">Response</span></span>
<span data-ttu-id="bc6a7-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc6a7-142">The following is an example of a response.</span></span>
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
