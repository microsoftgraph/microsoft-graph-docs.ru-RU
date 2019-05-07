---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 768e2a780fcfe96bd14d883d0f7ea0d03ac434cc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617093"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="c19e8-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="c19e8-103">Add directory role member</span></span>

<span data-ttu-id="c19e8-104">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="c19e8-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="c19e8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c19e8-105">Permissions</span></span>
<span data-ttu-id="c19e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19e8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c19e8-108">Permission type</span></span>      | <span data-ttu-id="c19e8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c19e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c19e8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c19e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c19e8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c19e8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c19e8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c19e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c19e8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19e8-113">Not supported.</span></span>    |
|<span data-ttu-id="c19e8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c19e8-114">Application</span></span> | <span data-ttu-id="c19e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c19e8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c19e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c19e8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c19e8-117">Request headers</span></span>
| <span data-ttu-id="c19e8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c19e8-118">Name</span></span>       | <span data-ttu-id="c19e8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c19e8-119">Type</span></span> | <span data-ttu-id="c19e8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c19e8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c19e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19e8-121">Authorization</span></span>  | <span data-ttu-id="c19e8-122">string</span><span class="sxs-lookup"><span data-stu-id="c19e8-122">string</span></span>  | <span data-ttu-id="c19e8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c19e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c19e8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c19e8-125">Content-Type</span></span>  | <span data-ttu-id="c19e8-126">string</span><span class="sxs-lookup"><span data-stu-id="c19e8-126">string</span></span>  | <span data-ttu-id="c19e8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c19e8-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c19e8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c19e8-128">Request body</span></span>
<span data-ttu-id="c19e8-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c19e8-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c19e8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19e8-130">Response</span></span>

<span data-ttu-id="c19e8-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c19e8-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c19e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c19e8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c19e8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c19e8-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="c19e8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19e8-134">Response</span></span>
<span data-ttu-id="c19e8-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c19e8-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c19e8-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c19e8-136">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c19e8-137">Язык</span><span class="sxs-lookup"><span data-stu-id="c19e8-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
