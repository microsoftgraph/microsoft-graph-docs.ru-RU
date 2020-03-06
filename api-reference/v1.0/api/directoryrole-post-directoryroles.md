---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ada6d1aba533ad8eeabbd4cbf64046f130711ff4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517932"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="dd77d-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="dd77d-106">Activate directoryRole</span></span>

<span data-ttu-id="dd77d-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd77d-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd77d-p102">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="dd77d-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd77d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd77d-112">Permissions</span></span>
<span data-ttu-id="dd77d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd77d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd77d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd77d-115">Permission type</span></span>      | <span data-ttu-id="dd77d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd77d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd77d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd77d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dd77d-118">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="dd77d-118">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd77d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd77d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd77d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd77d-120">Not supported.</span></span>    |
|<span data-ttu-id="dd77d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd77d-121">Application</span></span> | <span data-ttu-id="dd77d-122">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="dd77d-122">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd77d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd77d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="dd77d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd77d-124">Request headers</span></span>
| <span data-ttu-id="dd77d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dd77d-125">Name</span></span>       | <span data-ttu-id="dd77d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="dd77d-126">Type</span></span> | <span data-ttu-id="dd77d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="dd77d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd77d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd77d-128">Authorization</span></span>  | <span data-ttu-id="dd77d-129">string</span><span class="sxs-lookup"><span data-stu-id="dd77d-129">string</span></span>  | <span data-ttu-id="dd77d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd77d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd77d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd77d-132">Content-Type</span></span>  | <span data-ttu-id="dd77d-133">string</span><span class="sxs-lookup"><span data-stu-id="dd77d-133">string</span></span>  | <span data-ttu-id="dd77d-134">application/json</span><span class="sxs-lookup"><span data-stu-id="dd77d-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd77d-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd77d-135">Request body</span></span>
<span data-ttu-id="dd77d-136">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd77d-136">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="dd77d-137">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="dd77d-137">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="dd77d-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd77d-138">Parameter</span></span> | <span data-ttu-id="dd77d-139">Тип</span><span class="sxs-lookup"><span data-stu-id="dd77d-139">Type</span></span> | <span data-ttu-id="dd77d-140">Описание</span><span class="sxs-lookup"><span data-stu-id="dd77d-140">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="dd77d-141">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="dd77d-141">roleTemplateId</span></span> | <span data-ttu-id="dd77d-142">строка</span><span class="sxs-lookup"><span data-stu-id="dd77d-142">string</span></span> | <span data-ttu-id="dd77d-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd77d-143">Required.</span></span> <span data-ttu-id="dd77d-144">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="dd77d-144">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="dd77d-145">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="dd77d-145">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="dd77d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd77d-146">Response</span></span>

<span data-ttu-id="dd77d-147">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd77d-147">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd77d-148">Пример</span><span class="sxs-lookup"><span data-stu-id="dd77d-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd77d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd77d-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dd77d-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd77d-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd77d-151">C#</span><span class="sxs-lookup"><span data-stu-id="dd77d-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd77d-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd77d-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd77d-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd77d-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd77d-154">Java</span><span class="sxs-lookup"><span data-stu-id="dd77d-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dd77d-155">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd77d-155">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dd77d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd77d-156">Response</span></span>
<span data-ttu-id="dd77d-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd77d-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
