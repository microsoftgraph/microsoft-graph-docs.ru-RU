---
title: Активация directoryRole
description: Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только администраторы компании и роли каталога неявных пользователей. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b4c94d808185cb056a8481bdfbded071120fe42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434352"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="9f683-106">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="9f683-106">Activate directoryRole</span></span>

<span data-ttu-id="9f683-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f683-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f683-108">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="9f683-108">Activate a directory role.</span></span> <span data-ttu-id="9f683-109">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="9f683-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9f683-110">По умолчанию активируются только администраторы компании и роли каталога неявных пользователей.</span><span class="sxs-lookup"><span data-stu-id="9f683-110">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="9f683-111">Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="9f683-111">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f683-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f683-112">Permissions</span></span>
<span data-ttu-id="9f683-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f683-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f683-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f683-115">Permission type</span></span>      | <span data-ttu-id="9f683-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f683-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f683-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f683-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9f683-118">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9f683-118">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f683-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f683-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f683-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f683-120">Not supported.</span></span>    |
|<span data-ttu-id="9f683-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f683-121">Application</span></span> | <span data-ttu-id="9f683-122">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9f683-122">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f683-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f683-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="9f683-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f683-124">Request headers</span></span>
| <span data-ttu-id="9f683-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9f683-125">Name</span></span>       | <span data-ttu-id="9f683-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9f683-126">Type</span></span> | <span data-ttu-id="9f683-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9f683-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f683-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f683-128">Authorization</span></span>  | <span data-ttu-id="9f683-129">string</span><span class="sxs-lookup"><span data-stu-id="9f683-129">string</span></span>  | <span data-ttu-id="9f683-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f683-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f683-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f683-132">Request body</span></span>
<span data-ttu-id="9f683-133">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f683-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="9f683-134">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="9f683-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="9f683-135">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="9f683-135">Required parameter</span></span> | <span data-ttu-id="9f683-136">Тип</span><span class="sxs-lookup"><span data-stu-id="9f683-136">Type</span></span> | <span data-ttu-id="9f683-137">Описание</span><span class="sxs-lookup"><span data-stu-id="9f683-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="9f683-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9f683-138">roleTemplateId</span></span> | <span data-ttu-id="9f683-139">string</span><span class="sxs-lookup"><span data-stu-id="9f683-139">string</span></span> | <span data-ttu-id="9f683-p105">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="9f683-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="9f683-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f683-142">Response</span></span>

<span data-ttu-id="9f683-143">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f683-143">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f683-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9f683-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f683-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f683-145">Request</span></span>
<span data-ttu-id="9f683-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f683-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f683-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f683-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9f683-148">C#</span><span class="sxs-lookup"><span data-stu-id="9f683-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f683-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f683-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f683-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f683-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9f683-151">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f683-151">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f683-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f683-152">Response</span></span>
<span data-ttu-id="9f683-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f683-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
