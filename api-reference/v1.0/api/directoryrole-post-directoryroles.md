---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58c3560e40ccd2d5761cf9933e62b2df8f482d6a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373464"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="93226-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="93226-106">Activate directoryRole</span></span>

<span data-ttu-id="93226-p102">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="93226-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="93226-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93226-111">Permissions</span></span>
<span data-ttu-id="93226-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93226-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93226-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93226-114">Permission type</span></span>      | <span data-ttu-id="93226-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93226-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93226-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93226-116">Delegated (work or school account)</span></span> | <span data-ttu-id="93226-117">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="93226-117">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93226-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93226-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93226-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93226-119">Not supported.</span></span>    |
|<span data-ttu-id="93226-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93226-120">Application</span></span> | <span data-ttu-id="93226-121">Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="93226-121">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="93226-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93226-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="93226-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93226-123">Request headers</span></span>
| <span data-ttu-id="93226-124">Имя</span><span class="sxs-lookup"><span data-stu-id="93226-124">Name</span></span>       | <span data-ttu-id="93226-125">Тип</span><span class="sxs-lookup"><span data-stu-id="93226-125">Type</span></span> | <span data-ttu-id="93226-126">Описание</span><span class="sxs-lookup"><span data-stu-id="93226-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93226-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="93226-127">Authorization</span></span>  | <span data-ttu-id="93226-128">string</span><span class="sxs-lookup"><span data-stu-id="93226-128">string</span></span>  | <span data-ttu-id="93226-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93226-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93226-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93226-131">Content-Type</span></span>  | <span data-ttu-id="93226-132">string</span><span class="sxs-lookup"><span data-stu-id="93226-132">string</span></span>  | <span data-ttu-id="93226-133">application/json</span><span class="sxs-lookup"><span data-stu-id="93226-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93226-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93226-134">Request body</span></span>
<span data-ttu-id="93226-135">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93226-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="93226-136">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="93226-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="93226-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="93226-137">Parameter</span></span> | <span data-ttu-id="93226-138">Тип</span><span class="sxs-lookup"><span data-stu-id="93226-138">Type</span></span> | <span data-ttu-id="93226-139">Описание</span><span class="sxs-lookup"><span data-stu-id="93226-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="93226-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="93226-140">roleTemplateId</span></span> | <span data-ttu-id="93226-141">строка</span><span class="sxs-lookup"><span data-stu-id="93226-141">string</span></span> | <span data-ttu-id="93226-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93226-142">Required.</span></span> <span data-ttu-id="93226-143">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="93226-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="93226-144">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="93226-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="93226-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="93226-145">Response</span></span>

<span data-ttu-id="93226-146">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93226-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93226-147">Пример</span><span class="sxs-lookup"><span data-stu-id="93226-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93226-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="93226-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93226-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="93226-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="93226-150">C#</span><span class="sxs-lookup"><span data-stu-id="93226-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93226-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93226-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93226-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="93226-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="93226-153">Java</span><span class="sxs-lookup"><span data-stu-id="93226-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="93226-154">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93226-154">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="93226-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="93226-155">Response</span></span>
<span data-ttu-id="93226-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93226-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
