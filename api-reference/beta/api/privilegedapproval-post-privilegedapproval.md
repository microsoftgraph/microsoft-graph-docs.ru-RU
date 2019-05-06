---
title: Создание privilegedApproval
description: Используйте этот API для создания нового Привилежедаппровал.
localization_priority: Normal
ms.openlocfilehash: f07364cb37690de1236547909097343987f3cee0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595441"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="906f2-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="906f2-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906f2-104">Используйте этот API для создания нового Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="906f2-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="906f2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="906f2-105">Permissions</span></span>
<span data-ttu-id="906f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="906f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="906f2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="906f2-108">Permission type</span></span>      | <span data-ttu-id="906f2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="906f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="906f2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="906f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="906f2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="906f2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="906f2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="906f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="906f2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="906f2-113">Not supported.</span></span>    |
|<span data-ttu-id="906f2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="906f2-114">Application</span></span> | <span data-ttu-id="906f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="906f2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="906f2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="906f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="906f2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="906f2-117">Request headers</span></span>
| <span data-ttu-id="906f2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="906f2-118">Name</span></span>       | <span data-ttu-id="906f2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="906f2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="906f2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="906f2-120">Authorization</span></span>  | <span data-ttu-id="906f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="906f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="906f2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="906f2-123">Request body</span></span>
<span data-ttu-id="906f2-124">В тексте запроса добавьте представление объекта [Привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="906f2-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="906f2-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="906f2-125">Response</span></span>

<span data-ttu-id="906f2-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="906f2-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="906f2-127">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="906f2-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="906f2-128">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="906f2-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="906f2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="906f2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="906f2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="906f2-130">Request</span></span>
<span data-ttu-id="906f2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="906f2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="906f2-132">В тексте запроса добавьте представление объекта [Привилежедаппровал](../resources/privilegedapproval.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="906f2-132">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="906f2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="906f2-133">Response</span></span>
<span data-ttu-id="906f2-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="906f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="906f2-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="906f2-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="906f2-138">Языках</span><span class="sxs-lookup"><span data-stu-id="906f2-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="906f2-139">Язык</span><span class="sxs-lookup"><span data-stu-id="906f2-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
