---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8911b94d8f1ad5131a8299a3a1aa7be8365ab813
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181037"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="a2f6b-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="a2f6b-103">Permanently delete item</span></span>

<span data-ttu-id="a2f6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f6b-105">Окончательное удаление элемента из [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a2f6b-105">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a2f6b-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="a2f6b-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="a2f6b-107">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="a2f6b-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="a2f6b-108">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2f6b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f6b-109">Permissions</span></span>
<span data-ttu-id="a2f6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a2f6b-112">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="a2f6b-112">For applications:</span></span>

|<span data-ttu-id="a2f6b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f6b-113">Permission type</span></span>      | <span data-ttu-id="a2f6b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f6b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f6b-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2f6b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f6b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-118">Not supported.</span></span>    |
|<span data-ttu-id="a2f6b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2f6b-119">Application</span></span> | <span data-ttu-id="a2f6b-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="a2f6b-121">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="a2f6b-121">For users:</span></span>

|<span data-ttu-id="a2f6b-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f6b-122">Permission type</span></span>      | <span data-ttu-id="a2f6b-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f6b-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-124">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f6b-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a2f6b-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f6b-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-127">Not supported.</span></span> |
|<span data-ttu-id="a2f6b-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2f6b-128">Application</span></span> | <span data-ttu-id="a2f6b-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-129">User.ReadWrite.All</span></span> |

<span data-ttu-id="a2f6b-130">Для групп:</span><span class="sxs-lookup"><span data-stu-id="a2f6b-130">For groups:</span></span>

|<span data-ttu-id="a2f6b-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f6b-131">Permission type</span></span>      | <span data-ttu-id="a2f6b-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f6b-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-133">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f6b-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a2f6b-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2f6b-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f6b-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-136">Not supported.</span></span>    |
|<span data-ttu-id="a2f6b-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2f6b-137">Application</span></span> | <span data-ttu-id="a2f6b-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f6b-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2f6b-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2f6b-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a2f6b-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2f6b-140">Request headers</span></span>
| <span data-ttu-id="a2f6b-141">Имя</span><span class="sxs-lookup"><span data-stu-id="a2f6b-141">Name</span></span>       | <span data-ttu-id="a2f6b-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a2f6b-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2f6b-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2f6b-143">Authorization</span></span>  | <span data-ttu-id="a2f6b-144">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a2f6b-145">Accept</span><span class="sxs-lookup"><span data-stu-id="a2f6b-145">Accept</span></span>  | <span data-ttu-id="a2f6b-146">application/json</span><span class="sxs-lookup"><span data-stu-id="a2f6b-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2f6b-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2f6b-147">Request body</span></span>
<span data-ttu-id="a2f6b-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2f6b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2f6b-149">Response</span></span>

<span data-ttu-id="a2f6b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2f6b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a2f6b-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2f6b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2f6b-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a2f6b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f6b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="a2f6b-155">C#</span><span class="sxs-lookup"><span data-stu-id="a2f6b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2f6b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2f6b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2f6b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2f6b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2f6b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2f6b-158">Response</span></span>
<span data-ttu-id="a2f6b-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2f6b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
