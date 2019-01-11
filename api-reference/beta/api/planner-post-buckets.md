---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
ms.openlocfilehash: 06eeec8fd477ff57a89dfaa71eee262ac8f0be7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887880"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="28ff5-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="28ff5-103">Create plannerBucket</span></span>

> <span data-ttu-id="28ff5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="28ff5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28ff5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ff5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28ff5-106">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="28ff5-106">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ff5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28ff5-107">Permissions</span></span>
<span data-ttu-id="28ff5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ff5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28ff5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28ff5-110">Permission type</span></span>      | <span data-ttu-id="28ff5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28ff5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28ff5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28ff5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28ff5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ff5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28ff5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28ff5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ff5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ff5-115">Not supported.</span></span>    |
|<span data-ttu-id="28ff5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28ff5-116">Application</span></span> | <span data-ttu-id="28ff5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ff5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28ff5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28ff5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="28ff5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28ff5-119">Request headers</span></span>
| <span data-ttu-id="28ff5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="28ff5-120">Name</span></span>       | <span data-ttu-id="28ff5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="28ff5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28ff5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28ff5-122">Authorization</span></span>  | <span data-ttu-id="28ff5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28ff5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28ff5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28ff5-125">Request body</span></span>
<span data-ttu-id="28ff5-126">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28ff5-126">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="28ff5-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="28ff5-127">Response</span></span>

<span data-ttu-id="28ff5-128">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28ff5-128">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="28ff5-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="28ff5-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="28ff5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="28ff5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28ff5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ff5-133">Request</span></span>
<span data-ttu-id="28ff5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28ff5-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="28ff5-135">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28ff5-135">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="28ff5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="28ff5-136">Response</span></span>
<span data-ttu-id="28ff5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="28ff5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
