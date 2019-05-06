---
title: Обновление параметра каталога
description: Обновление свойств определенного объекта параметров каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d17abb40c6cf020b23be4fc0c319ebdee2684aa
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590269"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="6ee4d-103">Обновление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="6ee4d-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee4d-104">Обновление свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="6ee4d-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="6ee4d-106">Версия/v1.0 этого API была переименована для *обновления граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ee4d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee4d-107">Permissions</span></span>
<span data-ttu-id="6ee4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee4d-110">Permission type</span></span>      | <span data-ttu-id="6ee4d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ee4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ee4d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ee4d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ee4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-115">Not supported.</span></span>    |
|<span data-ttu-id="6ee4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ee4d-116">Application</span></span> | <span data-ttu-id="6ee4d-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee4d-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ee4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ee4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6ee4d-119">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6ee4d-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ee4d-120">Optional request headers</span></span>
| <span data-ttu-id="6ee4d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6ee4d-121">Name</span></span>       | <span data-ttu-id="6ee4d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ee4d-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6ee4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ee4d-123">Authorization</span></span>  | <span data-ttu-id="6ee4d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ee4d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ee4d-126">Request body</span></span>
<span data-ttu-id="6ee4d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="6ee4d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ee4d-128">Property</span></span>     | <span data-ttu-id="6ee4d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6ee4d-129">Type</span></span>   |<span data-ttu-id="6ee4d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6ee4d-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ee4d-131">values</span><span class="sxs-lookup"><span data-stu-id="6ee4d-131">values</span></span> | <span data-ttu-id="6ee4d-132">Коллекция [settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="6ee4d-p104">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="6ee4d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee4d-136">Response</span></span>

<span data-ttu-id="6ee4d-137">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ee4d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6ee4d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ee4d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee4d-139">Request</span></span>
<span data-ttu-id="6ee4d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6ee4d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee4d-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ee4d-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="6ee4d-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ee4d-143">Языках</span><span class="sxs-lookup"><span data-stu-id="6ee4d-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ee4d-144">Язык</span><span class="sxs-lookup"><span data-stu-id="6ee4d-144">Javascript</span></span>](#tab/javascript)
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
