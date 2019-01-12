---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5d642779f7ca179a6de485fae2caaafd065c050d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948354"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="a7cf4-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="a7cf4-103">Create plannerBucket</span></span>

<span data-ttu-id="a7cf4-104">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7cf4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7cf4-105">Permissions</span></span>
<span data-ttu-id="a7cf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7cf4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7cf4-108">Permission type</span></span>      | <span data-ttu-id="a7cf4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7cf4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7cf4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7cf4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7cf4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cf4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7cf4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7cf4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7cf4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-113">Not supported.</span></span>    |
|<span data-ttu-id="a7cf4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7cf4-114">Application</span></span> | <span data-ttu-id="a7cf4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7cf4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7cf4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="a7cf4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7cf4-117">Request headers</span></span>
| <span data-ttu-id="a7cf4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a7cf4-118">Name</span></span>       | <span data-ttu-id="a7cf4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a7cf4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7cf4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7cf4-120">Authorization</span></span>  | <span data-ttu-id="a7cf4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7cf4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7cf4-123">Request body</span></span>
<span data-ttu-id="a7cf4-124">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7cf4-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7cf4-125">Response</span></span>

<span data-ttu-id="a7cf4-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="a7cf4-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a7cf4-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a7cf4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7cf4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7cf4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7cf4-131">Request</span></span>
<span data-ttu-id="a7cf4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="a7cf4-133">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7cf4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7cf4-134">Response</span></span>
<span data-ttu-id="a7cf4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7cf4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
