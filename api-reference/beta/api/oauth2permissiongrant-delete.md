---
title: Удаление oAuth2PermissionGrant
description: Удаление oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 240462c1c20e3fc3d8ea55c95e348f6c7a7f53a7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597338"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="1676a-103">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1676a-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1676a-104">Удаление oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="1676a-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1676a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1676a-105">Permissions</span></span>
<span data-ttu-id="1676a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1676a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1676a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1676a-108">Permission type</span></span>      | <span data-ttu-id="1676a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1676a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1676a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1676a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1676a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1676a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1676a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1676a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1676a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1676a-113">Not supported.</span></span>    |
|<span data-ttu-id="1676a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1676a-114">Application</span></span> | <span data-ttu-id="1676a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1676a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1676a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1676a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1676a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1676a-117">Request headers</span></span>
| <span data-ttu-id="1676a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1676a-118">Name</span></span>       | <span data-ttu-id="1676a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1676a-119">Type</span></span> | <span data-ttu-id="1676a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1676a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1676a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1676a-121">Authorization</span></span>  | <span data-ttu-id="1676a-122">string</span><span class="sxs-lookup"><span data-stu-id="1676a-122">string</span></span>  | <span data-ttu-id="1676a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1676a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1676a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1676a-125">Request body</span></span>
<span data-ttu-id="1676a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1676a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1676a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1676a-127">Response</span></span>

<span data-ttu-id="1676a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1676a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1676a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1676a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1676a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1676a-131">Request</span></span>
<span data-ttu-id="1676a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1676a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="1676a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1676a-133">Response</span></span>
<span data-ttu-id="1676a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1676a-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1676a-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1676a-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1676a-136">Языках</span><span class="sxs-lookup"><span data-stu-id="1676a-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_oAuth2Permissiongrant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1676a-137">Язык</span><span class="sxs-lookup"><span data-stu-id="1676a-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_oAuth2Permissiongrant-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/oauth2permissiongrant-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
