---
title: Удаление Профилекардпроперти
description: Удаление объекта Профилекардпроперти и удаление всех настроек из карточки профиля.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2dffcc667281d26fb64e44dd7cd45e8e0f1c313f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080723"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="12da1-103">Удаление Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="12da1-103">Delete profileCardProperty</span></span>

<span data-ttu-id="12da1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12da1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12da1-105">Удалите объект [профилекардпроперти](../resources/profilecardproperty.md) , указанный в `directoryPropertyName` карточке профиля организации, и удалите все локализованные настройки для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="12da1-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="12da1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12da1-106">Permissions</span></span>

<span data-ttu-id="12da1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="12da1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="12da1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12da1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12da1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12da1-109">Permission type</span></span>                        | <span data-ttu-id="12da1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12da1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="12da1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12da1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12da1-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="12da1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="12da1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12da1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12da1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12da1-114">Not supported.</span></span>                              |
| <span data-ttu-id="12da1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12da1-115">Application</span></span>                            | <span data-ttu-id="12da1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12da1-116">Not supported.</span></span>                              |

><span data-ttu-id="12da1-117">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="12da1-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="12da1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12da1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="12da1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12da1-119">Request headers</span></span>

| <span data-ttu-id="12da1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="12da1-120">Name</span></span>          | <span data-ttu-id="12da1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="12da1-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="12da1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12da1-122">Authorization</span></span> | <span data-ttu-id="12da1-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="12da1-123">Bearer {token}.</span></span> <span data-ttu-id="12da1-124">Required.</span><span class="sxs-lookup"><span data-stu-id="12da1-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12da1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12da1-125">Request body</span></span>

<span data-ttu-id="12da1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12da1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12da1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="12da1-127">Response</span></span>

<span data-ttu-id="12da1-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="12da1-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="12da1-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="12da1-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12da1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="12da1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12da1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="12da1-131">Request</span></span>

<span data-ttu-id="12da1-132">В приведенном ниже примере показано, как удалить атрибут с именем "Fax" из карточки профиля для Организации.</span><span class="sxs-lookup"><span data-stu-id="12da1-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>

# <a name="http"></a>[<span data-ttu-id="12da1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="12da1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/fax
```
# <a name="c"></a>[<span data-ttu-id="12da1-134">C#</span><span class="sxs-lookup"><span data-stu-id="12da1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12da1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12da1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12da1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12da1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12da1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="12da1-137">Response</span></span>

<span data-ttu-id="12da1-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="12da1-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
