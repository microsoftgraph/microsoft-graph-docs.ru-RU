---
title: Активация directoryRole
description: Активация роли каталога.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: be7793024e9b8eb0f7ca9bec5a57d2b4ec1248db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448550"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="4b774-103">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="4b774-103">Activate directoryRole</span></span>

<span data-ttu-id="4b774-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b774-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b774-p101">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="4b774-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b774-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b774-109">Permissions</span></span>
<span data-ttu-id="4b774-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b774-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b774-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b774-112">Permission type</span></span>      | <span data-ttu-id="4b774-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b774-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b774-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b774-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4b774-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b774-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b774-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b774-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b774-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b774-117">Not supported.</span></span>    |
|<span data-ttu-id="4b774-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b774-118">Application</span></span> | <span data-ttu-id="4b774-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4b774-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b774-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b774-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="4b774-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b774-121">Request headers</span></span>
| <span data-ttu-id="4b774-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4b774-122">Name</span></span>       | <span data-ttu-id="4b774-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4b774-123">Type</span></span> | <span data-ttu-id="4b774-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4b774-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b774-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b774-125">Authorization</span></span>  | <span data-ttu-id="4b774-126">string</span><span class="sxs-lookup"><span data-stu-id="4b774-126">string</span></span>  | <span data-ttu-id="4b774-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b774-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b774-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b774-129">Content-Type</span></span>  | <span data-ttu-id="4b774-130">string</span><span class="sxs-lookup"><span data-stu-id="4b774-130">string</span></span>  | <span data-ttu-id="4b774-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4b774-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b774-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b774-132">Request body</span></span>
<span data-ttu-id="4b774-133">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b774-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="4b774-134">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4b774-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="4b774-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b774-135">Parameter</span></span> | <span data-ttu-id="4b774-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4b774-136">Type</span></span> | <span data-ttu-id="4b774-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4b774-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="4b774-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="4b774-138">roleTemplateId</span></span> | <span data-ttu-id="4b774-139">string</span><span class="sxs-lookup"><span data-stu-id="4b774-139">string</span></span> | <span data-ttu-id="4b774-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b774-140">Required.</span></span> <span data-ttu-id="4b774-141">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="4b774-141">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="4b774-142">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="4b774-142">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="4b774-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b774-143">Response</span></span>

<span data-ttu-id="4b774-144">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b774-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b774-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4b774-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b774-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b774-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4b774-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b774-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4b774-148">C#</span><span class="sxs-lookup"><span data-stu-id="4b774-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b774-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b774-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b774-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b774-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b774-151">Java</span><span class="sxs-lookup"><span data-stu-id="4b774-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4b774-152">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b774-152">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4b774-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b774-153">Response</span></span>
<span data-ttu-id="4b774-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b774-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
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

