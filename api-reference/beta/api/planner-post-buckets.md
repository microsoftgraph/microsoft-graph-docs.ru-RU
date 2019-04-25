---
title: Создание объекта plannerBucket
description: Используйте этот API, чтобы создать объект **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8baf98de9431c0627edfcf4adb8c04a16bc2a77f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539067"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="2addd-103">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2addd-103">Create plannerBucket</span></span>

<span data-ttu-id="2addd-104">Используйте этот API, чтобы создать объект **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="2addd-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2addd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2addd-105">Permissions</span></span>
<span data-ttu-id="2addd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2addd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2addd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2addd-108">Permission type</span></span>      | <span data-ttu-id="2addd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2addd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2addd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2addd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2addd-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2addd-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2addd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2addd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2addd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2addd-113">Not supported.</span></span>    |
|<span data-ttu-id="2addd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2addd-114">Application</span></span> | <span data-ttu-id="2addd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2addd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2addd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2addd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="2addd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2addd-117">Request headers</span></span>
| <span data-ttu-id="2addd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2addd-118">Name</span></span>       | <span data-ttu-id="2addd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2addd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2addd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2addd-120">Authorization</span></span>  | <span data-ttu-id="2addd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2addd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2addd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2addd-123">Request body</span></span>
<span data-ttu-id="2addd-124">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2addd-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2addd-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2addd-125">Response</span></span>

<span data-ttu-id="2addd-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2addd-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="2addd-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="2addd-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2addd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2addd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2addd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2addd-131">Request</span></span>
<span data-ttu-id="2addd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2addd-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="2addd-133">Включите в текст запроса описание объекта [plannerBucket](../resources/plannerbucket.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2addd-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2addd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2addd-134">Response</span></span>
<span data-ttu-id="2addd-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2addd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
