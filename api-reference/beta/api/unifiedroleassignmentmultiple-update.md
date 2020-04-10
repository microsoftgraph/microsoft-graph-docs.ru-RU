---
title: Обновление unifiedRoleAssignmentMultiple
description: Обновление нового объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a30e9378cceb5c1dd533f62bc28be097660536f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218964"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="a1aa1-103">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a1aa1-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="a1aa1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1aa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1aa1-105">Обновление существующего объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="a1aa1-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="a1aa1-106">Используйте эту возможность для обновления назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="a1aa1-107">Обратите внимание, что [унифиедролеассигнмент](../resources/unifiedroleassignment.md) не поддерживает обновление.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1aa1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1aa1-108">Permissions</span></span>

<span data-ttu-id="a1aa1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1aa1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1aa1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1aa1-111">Permission type</span></span> | <span data-ttu-id="a1aa1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="a1aa1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a1aa1-114">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a1aa1-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="a1aa1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1aa1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-116">Not supported.</span></span> |
| <span data-ttu-id="a1aa1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1aa1-117">Application</span></span> | <span data-ttu-id="a1aa1-118">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a1aa1-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1aa1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1aa1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a1aa1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1aa1-120">Request headers</span></span>

| <span data-ttu-id="a1aa1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a1aa1-121">Name</span></span> | <span data-ttu-id="a1aa1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a1aa1-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a1aa1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1aa1-123">Authorization</span></span> | <span data-ttu-id="a1aa1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1aa1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1aa1-126">Content-type</span></span> | <span data-ttu-id="a1aa1-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1aa1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1aa1-129">Request body</span></span>

<span data-ttu-id="a1aa1-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a1aa1-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a1aa1-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a1aa1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1aa1-133">Response</span></span>

<span data-ttu-id="a1aa1-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унифиедассигнментмултипле](../resources/unifiedroleassignmentMultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1aa1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a1aa1-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1aa1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1aa1-136">Request</span></span>

<span data-ttu-id="a1aa1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a1aa1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1aa1-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a1aa1-139">C#</span><span class="sxs-lookup"><span data-stu-id="a1aa1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1aa1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1aa1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1aa1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1aa1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1aa1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1aa1-142">Response</span></span>

<span data-ttu-id="a1aa1-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-143">The following is an example of the response.</span></span>
> <span data-ttu-id="a1aa1-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
