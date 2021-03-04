---
title: Обновление параметра каталога
description: Обновление свойств определенного объекта параметра каталога.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 805ad8068418d50e6cfc4a6e395a150782cb1aab
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436626"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="27035-103">Обновление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="27035-103">Update a directory setting</span></span>

<span data-ttu-id="27035-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27035-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27035-105">Обновление свойств определенного объекта параметра каталога.</span><span class="sxs-lookup"><span data-stu-id="27035-105">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="27035-106">**Примечание.** Бета-версия этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="27035-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="27035-107">Версия /v1.0 этого API переименована в *Update groupSettings.*</span><span class="sxs-lookup"><span data-stu-id="27035-107">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="27035-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27035-108">Permissions</span></span>
<span data-ttu-id="27035-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27035-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27035-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27035-111">Permission type</span></span>      | <span data-ttu-id="27035-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27035-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27035-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27035-113">Delegated (work or school account)</span></span> | <span data-ttu-id="27035-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27035-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27035-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27035-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27035-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27035-116">Not supported.</span></span>    |
|<span data-ttu-id="27035-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="27035-117">Application</span></span> | <span data-ttu-id="27035-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27035-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27035-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27035-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="27035-120">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="27035-120">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="27035-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27035-121">Optional request headers</span></span>
| <span data-ttu-id="27035-122">Имя</span><span class="sxs-lookup"><span data-stu-id="27035-122">Name</span></span>       | <span data-ttu-id="27035-123">Описание</span><span class="sxs-lookup"><span data-stu-id="27035-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="27035-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27035-124">Authorization</span></span>  | <span data-ttu-id="27035-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27035-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27035-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27035-127">Request body</span></span>
<span data-ttu-id="27035-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="27035-128">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="27035-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="27035-129">Property</span></span>     | <span data-ttu-id="27035-130">Тип</span><span class="sxs-lookup"><span data-stu-id="27035-130">Type</span></span>   |<span data-ttu-id="27035-131">Описание</span><span class="sxs-lookup"><span data-stu-id="27035-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27035-132">values</span><span class="sxs-lookup"><span data-stu-id="27035-132">values</span></span> | <span data-ttu-id="27035-133">[settingValue](../resources/settingvalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="27035-133">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="27035-p104">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="27035-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="27035-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="27035-137">Response</span></span>

<span data-ttu-id="27035-138">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="27035-138">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27035-139">Пример</span><span class="sxs-lookup"><span data-stu-id="27035-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27035-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="27035-140">Request</span></span>
<span data-ttu-id="27035-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27035-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27035-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="27035-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="27035-143">C#</span><span class="sxs-lookup"><span data-stu-id="27035-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27035-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27035-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27035-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27035-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27035-146">Java</span><span class="sxs-lookup"><span data-stu-id="27035-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27035-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="27035-147">Response</span></span>
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


