---
title: Создание владельца
description: Используйте этот API, чтобы создать нового владельца.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7ace73e1d6a2db3bac4502f9ddae6f4f0c0e1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856773"
---
# <a name="create-owner"></a><span data-ttu-id="82afd-103">Создание владельца</span><span class="sxs-lookup"><span data-stu-id="82afd-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82afd-104">Используйте этот API, чтобы создать нового владельца.</span><span class="sxs-lookup"><span data-stu-id="82afd-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="82afd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82afd-105">Permissions</span></span>
<span data-ttu-id="82afd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82afd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82afd-108">Permission type</span></span>      | <span data-ttu-id="82afd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82afd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82afd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82afd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="82afd-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82afd-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82afd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82afd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82afd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82afd-113">Not supported.</span></span>    |
|<span data-ttu-id="82afd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82afd-114">Application</span></span> | <span data-ttu-id="82afd-115">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="82afd-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82afd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82afd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="82afd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82afd-117">Request headers</span></span>
| <span data-ttu-id="82afd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="82afd-118">Name</span></span> | <span data-ttu-id="82afd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="82afd-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="82afd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82afd-120">Authorization</span></span> | <span data-ttu-id="82afd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82afd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82afd-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82afd-123">Request body</span></span>
<span data-ttu-id="82afd-124">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="82afd-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="82afd-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="82afd-125">Response</span></span>

<span data-ttu-id="82afd-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82afd-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82afd-127">Пример</span><span class="sxs-lookup"><span data-stu-id="82afd-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="82afd-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="82afd-128">Request</span></span>
<span data-ttu-id="82afd-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82afd-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82afd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="82afd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82afd-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="82afd-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="82afd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="82afd-132">Response</span></span>

<span data-ttu-id="82afd-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82afd-133">The following is an example of the response.</span></span>

><span data-ttu-id="82afd-134">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="82afd-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="82afd-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82afd-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
