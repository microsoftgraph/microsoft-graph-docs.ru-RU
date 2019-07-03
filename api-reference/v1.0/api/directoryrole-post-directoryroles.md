---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4044efdd467ea43569d7fd91052066a311f2ea42
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459316"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="f6840-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="f6840-106">Activate directoryRole</span></span>

<span data-ttu-id="f6840-p102">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="f6840-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6840-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6840-111">Permissions</span></span>
<span data-ttu-id="f6840-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6840-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6840-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6840-114">Permission type</span></span>      | <span data-ttu-id="f6840-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6840-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6840-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6840-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f6840-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6840-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6840-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6840-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6840-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6840-119">Not supported.</span></span>    |
|<span data-ttu-id="f6840-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6840-120">Application</span></span> | <span data-ttu-id="f6840-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6840-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6840-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6840-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="f6840-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6840-123">Request headers</span></span>
| <span data-ttu-id="f6840-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f6840-124">Name</span></span>       | <span data-ttu-id="f6840-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f6840-125">Type</span></span> | <span data-ttu-id="f6840-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f6840-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6840-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6840-127">Authorization</span></span>  | <span data-ttu-id="f6840-128">string</span><span class="sxs-lookup"><span data-stu-id="f6840-128">string</span></span>  | <span data-ttu-id="f6840-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6840-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6840-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6840-131">Content-Type</span></span>  | <span data-ttu-id="f6840-132">string</span><span class="sxs-lookup"><span data-stu-id="f6840-132">string</span></span>  | <span data-ttu-id="f6840-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f6840-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6840-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6840-134">Request body</span></span>
<span data-ttu-id="f6840-135">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6840-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="f6840-136">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="f6840-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="f6840-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="f6840-137">Parameter</span></span> | <span data-ttu-id="f6840-138">Тип</span><span class="sxs-lookup"><span data-stu-id="f6840-138">Type</span></span> | <span data-ttu-id="f6840-139">Описание</span><span class="sxs-lookup"><span data-stu-id="f6840-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="f6840-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="f6840-140">roleTemplateId</span></span> | <span data-ttu-id="f6840-141">строка</span><span class="sxs-lookup"><span data-stu-id="f6840-141">string</span></span> | <span data-ttu-id="f6840-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6840-142">Required.</span></span> <span data-ttu-id="f6840-143">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли.</span><span class="sxs-lookup"><span data-stu-id="f6840-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="f6840-144">Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="f6840-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="f6840-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6840-145">Response</span></span>

<span data-ttu-id="f6840-146">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f6840-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6840-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f6840-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6840-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6840-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f6840-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6840-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6840-150">C#</span><span class="sxs-lookup"><span data-stu-id="f6840-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6840-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6840-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6840-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6840-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f6840-153">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6840-153">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f6840-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6840-154">Response</span></span>
<span data-ttu-id="f6840-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6840-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
