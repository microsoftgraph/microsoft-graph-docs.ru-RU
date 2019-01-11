---
title: Получение synchronizationSchema
description: Получение схемы для задания синхронизации или шаблона.
localization_priority: Normal
ms.openlocfilehash: 768a35940593231bbc4fbd4c3f5498c7eb3243fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863471"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="c5fc6-103">Получение synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c5fc6-103">Get synchronizationSchema</span></span>

> <span data-ttu-id="c5fc6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5fc6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5fc6-106">Получение схемы для задания синхронизации или шаблона.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-106">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5fc6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5fc6-107">Permissions</span></span>
<span data-ttu-id="c5fc6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5fc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5fc6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5fc6-110">Permission type</span></span>                        | <span data-ttu-id="c5fc6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5fc6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5fc6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5fc6-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="c5fc6-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fc6-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c5fc6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5fc6-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c5fc6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-115">Not supported.</span></span> |
|<span data-ttu-id="c5fc6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5fc6-116">Application</span></span>                            |<span data-ttu-id="c5fc6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c5fc6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5fc6-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="c5fc6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5fc6-119">Request headers</span></span>

| <span data-ttu-id="c5fc6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c5fc6-120">Name</span></span>           | <span data-ttu-id="c5fc6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c5fc6-121">Type</span></span>    | <span data-ttu-id="c5fc6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c5fc6-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c5fc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fc6-123">Authorization</span></span>  | <span data-ttu-id="c5fc6-124">string</span><span class="sxs-lookup"><span data-stu-id="c5fc6-124">string</span></span>  | <span data-ttu-id="c5fc6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5fc6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5fc6-127">Request body</span></span>

<span data-ttu-id="c5fc6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5fc6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5fc6-129">Response</span></span>

<span data-ttu-id="c5fc6-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [synchronizationSchema](../resources/synchronization-synchronizationschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-130">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5fc6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c5fc6-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5fc6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5fc6-132">Request</span></span>
<span data-ttu-id="c5fc6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="c5fc6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5fc6-134">Response</span></span>
<span data-ttu-id="c5fc6-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-135">The following is an example of a response.</span></span>

><span data-ttu-id="c5fc6-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c5fc6-137">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="c5fc6-137">All the properties will be returned in an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
