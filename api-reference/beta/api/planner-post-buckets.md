---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 45745c40d28e1d9b4826178cc263af9b11bb9bed
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473670"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="2e228-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2e228-103">Create plannerBucket</span></span>

<span data-ttu-id="2e228-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e228-105">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="2e228-105">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e228-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e228-106">Permissions</span></span>
<span data-ttu-id="2e228-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e228-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e228-109">Permission type</span></span>      | <span data-ttu-id="2e228-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e228-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e228-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e228-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e228-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e228-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e228-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e228-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e228-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e228-114">Not supported.</span></span>    |
|<span data-ttu-id="2e228-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e228-115">Application</span></span> | <span data-ttu-id="2e228-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e228-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e228-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e228-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="2e228-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e228-118">Request headers</span></span>
| <span data-ttu-id="2e228-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e228-119">Name</span></span>       | <span data-ttu-id="2e228-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e228-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e228-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e228-121">Authorization</span></span>  | <span data-ttu-id="2e228-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e228-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e228-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e228-124">Request body</span></span>
<span data-ttu-id="2e228-125">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e228-125">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2e228-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e228-126">Response</span></span>

<span data-ttu-id="2e228-127">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e228-127">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="2e228-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="2e228-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2e228-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e228-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e228-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e228-132">Request</span></span>
<span data-ttu-id="2e228-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e228-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e228-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e228-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="c"></a>[<span data-ttu-id="2e228-135">C#</span><span class="sxs-lookup"><span data-stu-id="2e228-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e228-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e228-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e228-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e228-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e228-138">Java</span><span class="sxs-lookup"><span data-stu-id="2e228-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerbucket-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2e228-139">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e228-139">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2e228-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e228-140">Response</span></span>
<span data-ttu-id="2e228-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e228-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


