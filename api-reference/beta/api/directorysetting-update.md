---
title: Обновление параметра каталога
description: Обновление свойств определенного объекта параметров каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ccc01b1028f7822908859b78ba3fad41d5c6813
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321260"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="576da-103">Обновление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="576da-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="576da-104">Обновление свойств определенного объекта параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="576da-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="576da-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="576da-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="576da-106">Версия/v1.0 этого API была переименована для *обновления граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="576da-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="576da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="576da-107">Permissions</span></span>
<span data-ttu-id="576da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="576da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="576da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="576da-110">Permission type</span></span>      | <span data-ttu-id="576da-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="576da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="576da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="576da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="576da-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="576da-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="576da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="576da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="576da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="576da-115">Not supported.</span></span>    |
|<span data-ttu-id="576da-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="576da-116">Application</span></span> | <span data-ttu-id="576da-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="576da-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="576da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="576da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="576da-119">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="576da-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="576da-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="576da-120">Optional request headers</span></span>
| <span data-ttu-id="576da-121">Имя</span><span class="sxs-lookup"><span data-stu-id="576da-121">Name</span></span>       | <span data-ttu-id="576da-122">Описание</span><span class="sxs-lookup"><span data-stu-id="576da-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="576da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="576da-123">Authorization</span></span>  | <span data-ttu-id="576da-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="576da-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="576da-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="576da-126">Request body</span></span>
<span data-ttu-id="576da-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="576da-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="576da-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="576da-128">Property</span></span>     | <span data-ttu-id="576da-129">Тип</span><span class="sxs-lookup"><span data-stu-id="576da-129">Type</span></span>   |<span data-ttu-id="576da-130">Описание</span><span class="sxs-lookup"><span data-stu-id="576da-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="576da-131">values</span><span class="sxs-lookup"><span data-stu-id="576da-131">values</span></span> | <span data-ttu-id="576da-132">Коллекция [settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="576da-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="576da-p104">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="576da-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="576da-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="576da-136">Response</span></span>

<span data-ttu-id="576da-137">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="576da-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="576da-138">Пример</span><span class="sxs-lookup"><span data-stu-id="576da-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="576da-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="576da-139">Request</span></span>
<span data-ttu-id="576da-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="576da-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="576da-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="576da-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="576da-142">C#</span><span class="sxs-lookup"><span data-stu-id="576da-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="576da-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="576da-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="576da-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="576da-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="576da-145">Java</span><span class="sxs-lookup"><span data-stu-id="576da-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="576da-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="576da-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

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
  ]
}
-->
