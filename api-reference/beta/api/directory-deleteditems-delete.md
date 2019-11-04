---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7eb499efa6aca193ddcf4d641798c37f11c2d14b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937100"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="c5bc6-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="c5bc6-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5bc6-104">Окончательное удаление элемента из [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c5bc6-104">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="c5bc6-105">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="c5bc6-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="c5bc6-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="c5bc6-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="c5bc6-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5bc6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bc6-108">Permissions</span></span>
<span data-ttu-id="c5bc6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5bc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c5bc6-111">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="c5bc6-111">For applications:</span></span>

|<span data-ttu-id="c5bc6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bc6-112">Permission type</span></span>      | <span data-ttu-id="c5bc6-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5bc6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c5bc6-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5bc6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bc6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-117">Not supported.</span></span>    |
|<span data-ttu-id="c5bc6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5bc6-118">Application</span></span> | <span data-ttu-id="c5bc6-119">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-119">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="c5bc6-120">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="c5bc6-120">For users:</span></span>

|<span data-ttu-id="c5bc6-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bc6-121">Permission type</span></span>      | <span data-ttu-id="c5bc6-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5bc6-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-123">Delegated (work or school account)</span></span> | <span data-ttu-id="c5bc6-124">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-124">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c5bc6-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bc6-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-126">Not supported.</span></span> |
|<span data-ttu-id="c5bc6-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5bc6-127">Application</span></span> | <span data-ttu-id="c5bc6-128">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-128">User.ReadWrite.All</span></span> |

<span data-ttu-id="c5bc6-129">Для групп:</span><span class="sxs-lookup"><span data-stu-id="c5bc6-129">For groups:</span></span>

|<span data-ttu-id="c5bc6-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bc6-130">Permission type</span></span>      | <span data-ttu-id="c5bc6-131">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5bc6-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-132">Delegated (work or school account)</span></span> | <span data-ttu-id="c5bc6-133">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-133">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c5bc6-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bc6-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bc6-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-135">Not supported.</span></span>    |
|<span data-ttu-id="c5bc6-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5bc6-136">Application</span></span> | <span data-ttu-id="c5bc6-137">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bc6-137">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5bc6-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5bc6-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c5bc6-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5bc6-139">Request headers</span></span>
| <span data-ttu-id="c5bc6-140">Имя</span><span class="sxs-lookup"><span data-stu-id="c5bc6-140">Name</span></span>       | <span data-ttu-id="c5bc6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c5bc6-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5bc6-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5bc6-142">Authorization</span></span>  | <span data-ttu-id="c5bc6-143">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="c5bc6-144">Accept</span><span class="sxs-lookup"><span data-stu-id="c5bc6-144">Accept</span></span>  | <span data-ttu-id="c5bc6-145">application/json</span><span class="sxs-lookup"><span data-stu-id="c5bc6-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5bc6-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5bc6-146">Request body</span></span>
<span data-ttu-id="c5bc6-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5bc6-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5bc6-148">Response</span></span>

<span data-ttu-id="c5bc6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5bc6-151">Пример</span><span class="sxs-lookup"><span data-stu-id="c5bc6-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5bc6-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5bc6-152">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c5bc6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bc6-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5bc6-154">C#</span><span class="sxs-lookup"><span data-stu-id="c5bc6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5bc6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5bc6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5bc6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5bc6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5bc6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5bc6-157">Response</span></span>
<span data-ttu-id="c5bc6-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5bc6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
