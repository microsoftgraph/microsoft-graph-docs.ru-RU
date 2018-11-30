---
title: Обновление synchronizationSchema
description: Обновление схемы синхронизации для данного задания или шаблона. Этот метод полностью заменяет текущей схеме в запросе. Для обновления схемы шаблона, звонок на объект приложения. Необходимо быть владельцем приложения.
ms.openlocfilehash: 18ad164f0f1860ce954a9d4e1170f71e47f513b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080344"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="cb1ea-106">Обновление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="cb1ea-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="cb1ea-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb1ea-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb1ea-109">Обновление схемы синхронизации для данного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="cb1ea-110">Этот метод полностью заменяет текущей схеме в запросе.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="cb1ea-111">Для обновления схемы шаблона, звонок на объект приложения.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="cb1ea-112">Необходимо быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb1ea-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb1ea-113">Permissions</span></span>
<span data-ttu-id="cb1ea-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1ea-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb1ea-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb1ea-116">Permission type</span></span>                        | <span data-ttu-id="cb1ea-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb1ea-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb1ea-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb1ea-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="cb1ea-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb1ea-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cb1ea-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb1ea-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cb1ea-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-121">Not supported.</span></span>|
|<span data-ttu-id="cb1ea-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb1ea-122">Application</span></span>                            |<span data-ttu-id="cb1ea-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="cb1ea-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb1ea-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="cb1ea-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb1ea-125">Request headers</span></span>

| <span data-ttu-id="cb1ea-126">Имя</span><span class="sxs-lookup"><span data-stu-id="cb1ea-126">Name</span></span>           | <span data-ttu-id="cb1ea-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cb1ea-127">Type</span></span>    | <span data-ttu-id="cb1ea-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cb1ea-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cb1ea-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb1ea-129">Authorization</span></span>  | <span data-ttu-id="cb1ea-130">string</span><span class="sxs-lookup"><span data-stu-id="cb1ea-130">string</span></span>  | <span data-ttu-id="cb1ea-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb1ea-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb1ea-133">Request body</span></span>

<span data-ttu-id="cb1ea-134">В тексте запроса предоставить объект [synchronizationSchema](../resources/synchronization-synchronizationschema.md) для замены существующей схемы с.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="cb1ea-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb1ea-135">Response</span></span>

<span data-ttu-id="cb1ea-136">В случае успеха возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="cb1ea-137">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb1ea-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cb1ea-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cb1ea-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb1ea-139">Request</span></span>
<span data-ttu-id="cb1ea-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-140">The following is an example of a request.</span></span>

><span data-ttu-id="cb1ea-141">**Примечание:** Объект запроса, показанный сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="cb1ea-142">Предоставить все свойства фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-142">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cb1ea-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb1ea-143">Response</span></span>
<span data-ttu-id="cb1ea-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1ea-144">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->