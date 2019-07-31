---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только администраторы компании и роли каталога неявных пользователей. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef4e7ed1661309ea40a3a573fe5b830f65da7c88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957656"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="91d4f-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="91d4f-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d4f-107">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="91d4f-107">Activate a directory role.</span></span> <span data-ttu-id="91d4f-108">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="91d4f-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="91d4f-109">По умолчанию активируются только администраторы компании и роли каталога неявных пользователей.</span><span class="sxs-lookup"><span data-stu-id="91d4f-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="91d4f-110">Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="91d4f-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="91d4f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91d4f-111">Permissions</span></span>
<span data-ttu-id="91d4f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91d4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d4f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91d4f-114">Permission type</span></span>      | <span data-ttu-id="91d4f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91d4f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d4f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91d4f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="91d4f-117">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="91d4f-117">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91d4f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91d4f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d4f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91d4f-119">Not supported.</span></span>    |
|<span data-ttu-id="91d4f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91d4f-120">Application</span></span> | <span data-ttu-id="91d4f-121">Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="91d4f-121">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d4f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91d4f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="91d4f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91d4f-123">Request headers</span></span>
| <span data-ttu-id="91d4f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="91d4f-124">Name</span></span>       | <span data-ttu-id="91d4f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="91d4f-125">Type</span></span> | <span data-ttu-id="91d4f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="91d4f-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91d4f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d4f-127">Authorization</span></span>  | <span data-ttu-id="91d4f-128">string</span><span class="sxs-lookup"><span data-stu-id="91d4f-128">string</span></span>  | <span data-ttu-id="91d4f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91d4f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91d4f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91d4f-131">Request body</span></span>
<span data-ttu-id="91d4f-132">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91d4f-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="91d4f-133">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="91d4f-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="91d4f-134">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="91d4f-134">Required parameter</span></span> | <span data-ttu-id="91d4f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="91d4f-135">Type</span></span> | <span data-ttu-id="91d4f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="91d4f-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="91d4f-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="91d4f-137">roleTemplateId</span></span> | <span data-ttu-id="91d4f-138">string</span><span class="sxs-lookup"><span data-stu-id="91d4f-138">string</span></span> | <span data-ttu-id="91d4f-p105">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="91d4f-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="91d4f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91d4f-141">Response</span></span>

<span data-ttu-id="91d4f-142">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91d4f-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d4f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="91d4f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91d4f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="91d4f-144">Request</span></span>
<span data-ttu-id="91d4f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91d4f-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91d4f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="91d4f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91d4f-147">C#</span><span class="sxs-lookup"><span data-stu-id="91d4f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91d4f-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="91d4f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91d4f-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="91d4f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="91d4f-150">Java</span><span class="sxs-lookup"><span data-stu-id="91d4f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="91d4f-151">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91d4f-151">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="91d4f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="91d4f-152">Response</span></span>
<span data-ttu-id="91d4f-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91d4f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
