---
title: Обновление unifiedRoleAssignmentMultiple
description: Обновление нового объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5bd8485a9b01890420d47e95d976b84b0807b488
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054751"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="4e623-103">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="4e623-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="4e623-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e623-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e623-105">Обновление [существующего объекта unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="4e623-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="4e623-106">Используйте это для обновления назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4e623-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="4e623-107">Обратите [внимание, что unifiedRoleAssignment](../resources/unifiedroleassignment.md) не поддерживает обновление.</span><span class="sxs-lookup"><span data-stu-id="4e623-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e623-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e623-108">Permissions</span></span>

<span data-ttu-id="4e623-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e623-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e623-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e623-111">Permission type</span></span> | <span data-ttu-id="4e623-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e623-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="4e623-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e623-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4e623-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e623-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="4e623-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e623-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e623-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e623-116">Not supported.</span></span> |
| <span data-ttu-id="4e623-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e623-117">Application</span></span> | <span data-ttu-id="4e623-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e623-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e623-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e623-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="4e623-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e623-120">Request headers</span></span>

| <span data-ttu-id="4e623-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4e623-121">Name</span></span> | <span data-ttu-id="4e623-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4e623-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="4e623-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e623-123">Authorization</span></span> | <span data-ttu-id="4e623-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e623-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e623-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e623-126">Content-type</span></span> | <span data-ttu-id="4e623-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e623-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e623-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e623-129">Request body</span></span>

<span data-ttu-id="4e623-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4e623-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4e623-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4e623-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4e623-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4e623-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4e623-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e623-133">Response</span></span>

<span data-ttu-id="4e623-134">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e623-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e623-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4e623-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e623-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e623-136">Request</span></span>

<span data-ttu-id="4e623-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e623-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e623-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e623-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[<span data-ttu-id="4e623-139">C#</span><span class="sxs-lookup"><span data-stu-id="4e623-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e623-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e623-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e623-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e623-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e623-142">Java</span><span class="sxs-lookup"><span data-stu-id="4e623-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4e623-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e623-143">Response</span></span>

<span data-ttu-id="4e623-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4e623-144">The following is an example of the response.</span></span>
> <span data-ttu-id="4e623-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4e623-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 204 OK

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


