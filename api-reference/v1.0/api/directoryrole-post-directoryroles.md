---
title: Активация directoryRole
description: Активация роли каталога.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7078b50b05f521d5940cef69565025c5fbf66f21
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854133"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="b3fcc-103">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="b3fcc-103">Activate directoryRole</span></span>

<span data-ttu-id="b3fcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3fcc-p101">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="b3fcc-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3fcc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3fcc-109">Permissions</span></span>
<span data-ttu-id="b3fcc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3fcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3fcc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3fcc-112">Permission type</span></span>      | <span data-ttu-id="b3fcc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3fcc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3fcc-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3fcc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b3fcc-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3fcc-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3fcc-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3fcc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3fcc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-117">Not supported.</span></span>    |
|<span data-ttu-id="b3fcc-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3fcc-118">Application</span></span> | <span data-ttu-id="b3fcc-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="b3fcc-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3fcc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3fcc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="b3fcc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3fcc-121">Request headers</span></span>
| <span data-ttu-id="b3fcc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b3fcc-122">Name</span></span>       | <span data-ttu-id="b3fcc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b3fcc-123">Type</span></span> | <span data-ttu-id="b3fcc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b3fcc-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3fcc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3fcc-125">Authorization</span></span>  | <span data-ttu-id="b3fcc-126">string</span><span class="sxs-lookup"><span data-stu-id="b3fcc-126">string</span></span>  | <span data-ttu-id="b3fcc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3fcc-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3fcc-129">Content-Type</span></span>  | <span data-ttu-id="b3fcc-130">string</span><span class="sxs-lookup"><span data-stu-id="b3fcc-130">string</span></span>  | <span data-ttu-id="b3fcc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b3fcc-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3fcc-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3fcc-132">Request body</span></span>
<span data-ttu-id="b3fcc-133">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="b3fcc-134">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="b3fcc-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3fcc-135">Parameter</span></span> | <span data-ttu-id="b3fcc-136">Тип</span><span class="sxs-lookup"><span data-stu-id="b3fcc-136">Type</span></span> | <span data-ttu-id="b3fcc-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b3fcc-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="b3fcc-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="b3fcc-138">roleTemplateId</span></span> | <span data-ttu-id="b3fcc-139">string</span><span class="sxs-lookup"><span data-stu-id="b3fcc-139">string</span></span> | <span data-ttu-id="b3fcc-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-140">Required.</span></span> <span data-ttu-id="b3fcc-141">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-141">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="b3fcc-142">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-142">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="b3fcc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3fcc-143">Response</span></span>

<span data-ttu-id="b3fcc-144">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3fcc-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b3fcc-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3fcc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3fcc-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b3fcc-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3fcc-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
}
```
# <a name="c"></a>[<span data-ttu-id="b3fcc-148">C#</span><span class="sxs-lookup"><span data-stu-id="b3fcc-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3fcc-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3fcc-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3fcc-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3fcc-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3fcc-151">Java</span><span class="sxs-lookup"><span data-stu-id="b3fcc-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b3fcc-152">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-152">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b3fcc-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3fcc-153">Response</span></span>
<span data-ttu-id="b3fcc-154">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3fcc-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
  "id": "76f84d30-2759-4c66-915d-65c6e4083fa0",
  "deletedDateTime": null,
  "description": "Can manage all aspects of users and groups, including resetting passwords for limited admins.",
  "displayName": "User Administrator",
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

