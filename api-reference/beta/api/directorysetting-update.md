---
title: Обновление параметра каталога
description: Обновление свойств определенного объекта параметров каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba33e86046443d0af573a0a7f62125cc4b419f24
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655819"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="cc530-103">Обновление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="cc530-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc530-104">Обновление свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="cc530-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="cc530-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="cc530-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="cc530-106">Версия/v1.0 этого API была переименована для *обновления граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="cc530-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc530-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc530-107">Permissions</span></span>
<span data-ttu-id="cc530-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc530-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc530-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc530-110">Permission type</span></span>      | <span data-ttu-id="cc530-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc530-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc530-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc530-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc530-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc530-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc530-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc530-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc530-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc530-115">Not supported.</span></span>    |
|<span data-ttu-id="cc530-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc530-116">Application</span></span> | <span data-ttu-id="cc530-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc530-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc530-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc530-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cc530-119">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="cc530-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cc530-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc530-120">Optional request headers</span></span>
| <span data-ttu-id="cc530-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cc530-121">Name</span></span>       | <span data-ttu-id="cc530-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cc530-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cc530-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc530-123">Authorization</span></span>  | <span data-ttu-id="cc530-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc530-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc530-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc530-126">Request body</span></span>
<span data-ttu-id="cc530-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cc530-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="cc530-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc530-128">Property</span></span>     | <span data-ttu-id="cc530-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cc530-129">Type</span></span>   |<span data-ttu-id="cc530-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cc530-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc530-131">values</span><span class="sxs-lookup"><span data-stu-id="cc530-131">values</span></span> | <span data-ttu-id="cc530-132">Коллекция [settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cc530-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="cc530-p104">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="cc530-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="cc530-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc530-136">Response</span></span>

<span data-ttu-id="cc530-137">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="cc530-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cc530-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cc530-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc530-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc530-139">Request</span></span>
<span data-ttu-id="cc530-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc530-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="cc530-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc530-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cc530-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="cc530-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cc530-143">C#</span><span class="sxs-lookup"><span data-stu-id="cc530-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc530-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc530-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_directorysetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
