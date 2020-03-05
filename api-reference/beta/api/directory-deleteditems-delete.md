---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2cbee272810cf58b48e1a28cb1559bfe382b27dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435530"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="6f9df-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="6f9df-103">Permanently delete item</span></span>

<span data-ttu-id="6f9df-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f9df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f9df-105">Окончательное удаление элемента из [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6f9df-105">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="6f9df-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="6f9df-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="6f9df-107">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="6f9df-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="6f9df-108">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="6f9df-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f9df-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9df-109">Permissions</span></span>
<span data-ttu-id="6f9df-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f9df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6f9df-112">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="6f9df-112">For applications:</span></span>

|<span data-ttu-id="6f9df-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9df-113">Permission type</span></span>      | <span data-ttu-id="6f9df-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f9df-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f9df-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f9df-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6f9df-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f9df-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f9df-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f9df-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f9df-118">Not supported.</span></span>    |
|<span data-ttu-id="6f9df-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f9df-119">Application</span></span> | <span data-ttu-id="6f9df-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="6f9df-121">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="6f9df-121">For users:</span></span>

|<span data-ttu-id="6f9df-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9df-122">Permission type</span></span>      | <span data-ttu-id="6f9df-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f9df-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f9df-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f9df-124">Delegated (work or school account)</span></span> | <span data-ttu-id="6f9df-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6f9df-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f9df-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f9df-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f9df-127">Not supported.</span></span> |
|<span data-ttu-id="6f9df-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f9df-128">Application</span></span> | <span data-ttu-id="6f9df-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-129">User.ReadWrite.All</span></span> |

<span data-ttu-id="6f9df-130">Для групп:</span><span class="sxs-lookup"><span data-stu-id="6f9df-130">For groups:</span></span>

|<span data-ttu-id="6f9df-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9df-131">Permission type</span></span>      | <span data-ttu-id="6f9df-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f9df-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f9df-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f9df-133">Delegated (work or school account)</span></span> | <span data-ttu-id="6f9df-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6f9df-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f9df-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f9df-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f9df-136">Not supported.</span></span>    |
|<span data-ttu-id="6f9df-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f9df-137">Application</span></span> | <span data-ttu-id="6f9df-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9df-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f9df-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f9df-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6f9df-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f9df-140">Request headers</span></span>
| <span data-ttu-id="6f9df-141">Имя</span><span class="sxs-lookup"><span data-stu-id="6f9df-141">Name</span></span>       | <span data-ttu-id="6f9df-142">Описание</span><span class="sxs-lookup"><span data-stu-id="6f9df-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f9df-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f9df-143">Authorization</span></span>  | <span data-ttu-id="6f9df-144">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="6f9df-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="6f9df-145">Accept</span><span class="sxs-lookup"><span data-stu-id="6f9df-145">Accept</span></span>  | <span data-ttu-id="6f9df-146">application/json</span><span class="sxs-lookup"><span data-stu-id="6f9df-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f9df-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f9df-147">Request body</span></span>
<span data-ttu-id="6f9df-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f9df-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f9df-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f9df-149">Response</span></span>

<span data-ttu-id="6f9df-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6f9df-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f9df-152">Пример</span><span class="sxs-lookup"><span data-stu-id="6f9df-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f9df-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f9df-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6f9df-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f9df-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="6f9df-155">C#</span><span class="sxs-lookup"><span data-stu-id="6f9df-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f9df-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f9df-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f9df-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f9df-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f9df-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f9df-158">Response</span></span>
<span data-ttu-id="6f9df-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f9df-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
