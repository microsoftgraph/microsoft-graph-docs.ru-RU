---
title: Назначение соединителиГрупп приложению
description: Использование этого API для назначения соединителиГрупп приложению
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1c117153bff6ee7864eb174c38014f4adc939dee
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129571"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="92762-103">Назначение соединителиГрупп приложению</span><span class="sxs-lookup"><span data-stu-id="92762-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="92762-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92762-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92762-105">[Назначьте соединителиГрупп](../resources/connectorgroup.md) [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="92762-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92762-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92762-106">Permissions</span></span>
<span data-ttu-id="92762-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92762-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92762-109">Permission type</span></span>      | <span data-ttu-id="92762-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92762-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92762-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92762-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92762-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92762-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92762-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92762-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92762-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92762-114">Not supported.</span></span>    |
|<span data-ttu-id="92762-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92762-115">Application</span></span> | <span data-ttu-id="92762-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92762-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="92762-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92762-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="92762-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92762-118">Request headers</span></span>
| <span data-ttu-id="92762-119">Имя</span><span class="sxs-lookup"><span data-stu-id="92762-119">Name</span></span>       | <span data-ttu-id="92762-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92762-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92762-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92762-121">Authorization</span></span>  | <span data-ttu-id="92762-122">Bearer.</span><span class="sxs-lookup"><span data-stu-id="92762-122">Bearer.</span></span> <span data-ttu-id="92762-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="92762-123">Required.</span></span>|
| <span data-ttu-id="92762-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92762-124">Content-type</span></span> | <span data-ttu-id="92762-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92762-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92762-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92762-127">Request body</span></span>
<span data-ttu-id="92762-128">В теле запроса укажет представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="92762-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92762-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="92762-129">Response</span></span>

<span data-ttu-id="92762-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92762-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92762-131">Пример</span><span class="sxs-lookup"><span data-stu-id="92762-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="92762-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="92762-132">Request</span></span>
<span data-ttu-id="92762-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92762-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92762-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="92762-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="92762-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92762-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="92762-136">C#</span><span class="sxs-lookup"><span data-stu-id="92762-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92762-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92762-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92762-138">Java</span><span class="sxs-lookup"><span data-stu-id="92762-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92762-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="92762-139">Response</span></span>
<span data-ttu-id="92762-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92762-140">The following is an example of the response.</span></span> 

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



