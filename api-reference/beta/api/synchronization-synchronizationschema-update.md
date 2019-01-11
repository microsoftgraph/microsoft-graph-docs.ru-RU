---
title: Обновление synchronizationSchema
description: Обновление схемы синхронизации для данного задания или шаблона. Этот метод полностью заменяет текущей схеме в запросе. Для обновления схемы шаблона, звонок на объект приложения. Необходимо быть владельцем приложения.
localization_priority: Normal
ms.openlocfilehash: d4f3f3540fe0d304b4edc3a5fcaec7b3366dbb0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826140"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="1cce6-106">Обновление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1cce6-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="1cce6-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cce6-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cce6-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cce6-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cce6-109">Обновление схемы синхронизации для данного задания или шаблона.</span><span class="sxs-lookup"><span data-stu-id="1cce6-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="1cce6-110">Этот метод полностью заменяет текущей схеме в запросе.</span><span class="sxs-lookup"><span data-stu-id="1cce6-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="1cce6-111">Для обновления схемы шаблона, звонок на объект приложения.</span><span class="sxs-lookup"><span data-stu-id="1cce6-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="1cce6-112">Необходимо быть владельцем приложения.</span><span class="sxs-lookup"><span data-stu-id="1cce6-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cce6-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cce6-113">Permissions</span></span>
<span data-ttu-id="1cce6-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cce6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cce6-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cce6-116">Permission type</span></span>                        | <span data-ttu-id="1cce6-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cce6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cce6-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cce6-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="1cce6-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cce6-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1cce6-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cce6-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1cce6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cce6-121">Not supported.</span></span>|
|<span data-ttu-id="1cce6-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cce6-122">Application</span></span>                            |<span data-ttu-id="1cce6-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cce6-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="1cce6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cce6-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="1cce6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cce6-125">Request headers</span></span>

| <span data-ttu-id="1cce6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="1cce6-126">Name</span></span>           | <span data-ttu-id="1cce6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1cce6-127">Type</span></span>    | <span data-ttu-id="1cce6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1cce6-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1cce6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cce6-129">Authorization</span></span>  | <span data-ttu-id="1cce6-130">string</span><span class="sxs-lookup"><span data-stu-id="1cce6-130">string</span></span>  | <span data-ttu-id="1cce6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cce6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cce6-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cce6-133">Request body</span></span>

<span data-ttu-id="1cce6-134">В тексте запроса предоставить объект [synchronizationSchema](../resources/synchronization-synchronizationschema.md) для замены существующей схемы с.</span><span class="sxs-lookup"><span data-stu-id="1cce6-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="1cce6-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cce6-135">Response</span></span>

<span data-ttu-id="1cce6-136">В случае успеха возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="1cce6-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="1cce6-137">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1cce6-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cce6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1cce6-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1cce6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cce6-139">Request</span></span>
<span data-ttu-id="1cce6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cce6-140">The following is an example of a request.</span></span>

><span data-ttu-id="1cce6-141">**Примечание:** Объект запроса, показанный сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1cce6-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="1cce6-142">Предоставить все свойства фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="1cce6-142">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1cce6-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cce6-143">Response</span></span>
<span data-ttu-id="1cce6-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1cce6-144">The following is an example of a response.</span></span>
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
