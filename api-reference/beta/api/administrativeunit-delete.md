---
title: Удаление administrativeUnit
description: Удаление administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fd7b23911c1c42bb98da397f8775dd6f73512d5a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636767"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="5da9e-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5da9e-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5da9e-104">Удаление [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="5da9e-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5da9e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5da9e-105">Permissions</span></span>
<span data-ttu-id="5da9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5da9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5da9e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5da9e-108">Permission type</span></span>      | <span data-ttu-id="5da9e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5da9e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5da9e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5da9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5da9e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5da9e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5da9e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5da9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5da9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5da9e-113">Not supported.</span></span>    |
|<span data-ttu-id="5da9e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5da9e-114">Application</span></span> | <span data-ttu-id="5da9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5da9e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5da9e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5da9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5da9e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5da9e-117">Request headers</span></span>
| <span data-ttu-id="5da9e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5da9e-118">Name</span></span>       | <span data-ttu-id="5da9e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5da9e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5da9e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5da9e-120">Authorization</span></span>  | <span data-ttu-id="5da9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5da9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5da9e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5da9e-123">Request body</span></span>
<span data-ttu-id="5da9e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5da9e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5da9e-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="5da9e-125">Response</span></span>

<span data-ttu-id="5da9e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5da9e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5da9e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5da9e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5da9e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5da9e-129">Request</span></span>
<span data-ttu-id="5da9e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5da9e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="5da9e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5da9e-131">Response</span></span>
<span data-ttu-id="5da9e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5da9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5da9e-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5da9e-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5da9e-136">Языках</span><span class="sxs-lookup"><span data-stu-id="5da9e-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5da9e-137">Язык</span><span class="sxs-lookup"><span data-stu-id="5da9e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
