---
title: Назначение соединителиГрупп приложению
description: Использование этого API для назначения соединителиГрупп приложению
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 467320f0118743a29415a035421c4a92496aaf38
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752875"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="335c1-103">Назначение соединителиГрупп приложению</span><span class="sxs-lookup"><span data-stu-id="335c1-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="335c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="335c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="335c1-105">[Назначьте соединителиГрупп](../resources/connectorgroup.md) [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="335c1-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="335c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="335c1-106">Permissions</span></span>
<span data-ttu-id="335c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="335c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="335c1-109">Permission type</span></span>      | <span data-ttu-id="335c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="335c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="335c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="335c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="335c1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="335c1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="335c1-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="335c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="335c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="335c1-114">Not supported.</span></span>    |
|<span data-ttu-id="335c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="335c1-115">Application</span></span> | <span data-ttu-id="335c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="335c1-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="335c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="335c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="335c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="335c1-118">Request headers</span></span>
| <span data-ttu-id="335c1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="335c1-119">Name</span></span>       | <span data-ttu-id="335c1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="335c1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="335c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="335c1-121">Authorization</span></span>  | <span data-ttu-id="335c1-122">Bearer.</span><span class="sxs-lookup"><span data-stu-id="335c1-122">Bearer.</span></span> <span data-ttu-id="335c1-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="335c1-123">Required.</span></span>|
| <span data-ttu-id="335c1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="335c1-124">Content-type</span></span> | <span data-ttu-id="335c1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="335c1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="335c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="335c1-127">Request body</span></span>
<span data-ttu-id="335c1-128">В теле запроса укажете представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="335c1-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="335c1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="335c1-129">Response</span></span>

<span data-ttu-id="335c1-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="335c1-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="335c1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="335c1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="335c1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="335c1-132">Request</span></span>
<span data-ttu-id="335c1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="335c1-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="335c1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="335c1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/connectorGroup/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="335c1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="335c1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="335c1-136">C#</span><span class="sxs-lookup"><span data-stu-id="335c1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="335c1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="335c1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="335c1-138">Java</span><span class="sxs-lookup"><span data-stu-id="335c1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="335c1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="335c1-139">Response</span></span>
<span data-ttu-id="335c1-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="335c1-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Assign a connectorGroup to an application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


