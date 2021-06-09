---
title: Активация directoryRole
description: Активация роли каталога.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a9cc827495345c4a08eff75a4baa53603ab29177
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854216"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="73d60-103">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="73d60-103">Activate directoryRole</span></span>

<span data-ttu-id="73d60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d60-105">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="73d60-105">Activate a directory role.</span></span> <span data-ttu-id="73d60-106">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="73d60-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="73d60-107">По умолчанию активируются только администраторы компании и неявные роли каталога пользователей.</span><span class="sxs-lookup"><span data-stu-id="73d60-107">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="73d60-108">Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="73d60-108">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="73d60-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73d60-109">Permissions</span></span>
<span data-ttu-id="73d60-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d60-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73d60-112">Permission type</span></span>      | <span data-ttu-id="73d60-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73d60-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73d60-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73d60-114">Delegated (work or school account)</span></span> | <span data-ttu-id="73d60-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73d60-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73d60-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73d60-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d60-117">Not supported.</span></span>    |
|<span data-ttu-id="73d60-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="73d60-118">Application</span></span> | <span data-ttu-id="73d60-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="73d60-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="73d60-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73d60-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="73d60-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73d60-121">Request headers</span></span>
| <span data-ttu-id="73d60-122">Имя</span><span class="sxs-lookup"><span data-stu-id="73d60-122">Name</span></span>       | <span data-ttu-id="73d60-123">Тип</span><span class="sxs-lookup"><span data-stu-id="73d60-123">Type</span></span> | <span data-ttu-id="73d60-124">Описание</span><span class="sxs-lookup"><span data-stu-id="73d60-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73d60-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d60-125">Authorization</span></span>  | <span data-ttu-id="73d60-126">string</span><span class="sxs-lookup"><span data-stu-id="73d60-126">string</span></span>  | <span data-ttu-id="73d60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73d60-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73d60-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73d60-129">Request body</span></span>
<span data-ttu-id="73d60-130">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73d60-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="73d60-131">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="73d60-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="73d60-132">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="73d60-132">Required parameter</span></span> | <span data-ttu-id="73d60-133">Тип</span><span class="sxs-lookup"><span data-stu-id="73d60-133">Type</span></span> | <span data-ttu-id="73d60-134">Описание</span><span class="sxs-lookup"><span data-stu-id="73d60-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="73d60-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="73d60-135">roleTemplateId</span></span> | <span data-ttu-id="73d60-136">string</span><span class="sxs-lookup"><span data-stu-id="73d60-136">string</span></span> | <span data-ttu-id="73d60-p104">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="73d60-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="73d60-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d60-139">Response</span></span>

<span data-ttu-id="73d60-140">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73d60-140">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d60-141">Пример</span><span class="sxs-lookup"><span data-stu-id="73d60-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73d60-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="73d60-142">Request</span></span>
<span data-ttu-id="73d60-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73d60-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73d60-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d60-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
}
```
# <a name="c"></a>[<span data-ttu-id="73d60-145">C#</span><span class="sxs-lookup"><span data-stu-id="73d60-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73d60-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d60-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d60-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d60-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d60-148">Java</span><span class="sxs-lookup"><span data-stu-id="73d60-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="73d60-149">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73d60-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="73d60-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d60-150">Response</span></span>
<span data-ttu-id="73d60-p105">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73d60-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
  "id": "76f84d30-2759-4c66-915d-65c6e4083fa0",
  "deletedDateTime": null,
  "description": "Can manage all aspects of users and groups, including resetting passwords for limited admins.",
  "displayName": "User Administrator",
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
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


