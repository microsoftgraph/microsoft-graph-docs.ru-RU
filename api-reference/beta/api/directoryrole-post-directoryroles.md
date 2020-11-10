---
title: Активация directoryRole
description: Активация роли каталога.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 221d7b26f7488d925602be4550e5a7fe372f6bea
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956331"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="a748a-103">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="a748a-103">Activate directoryRole</span></span>

<span data-ttu-id="a748a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a748a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a748a-105">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a748a-105">Activate a directory role.</span></span> <span data-ttu-id="a748a-106">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="a748a-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="a748a-107">По умолчанию активируются только администраторы компании и роли каталога неявных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a748a-107">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="a748a-108">Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="a748a-108">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a748a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a748a-109">Permissions</span></span>
<span data-ttu-id="a748a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a748a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a748a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a748a-112">Permission type</span></span>      | <span data-ttu-id="a748a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a748a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a748a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a748a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a748a-115">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a748a-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a748a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a748a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a748a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a748a-117">Not supported.</span></span>    |
|<span data-ttu-id="a748a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a748a-118">Application</span></span> | <span data-ttu-id="a748a-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a748a-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a748a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a748a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="a748a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a748a-121">Request headers</span></span>
| <span data-ttu-id="a748a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a748a-122">Name</span></span>       | <span data-ttu-id="a748a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a748a-123">Type</span></span> | <span data-ttu-id="a748a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a748a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a748a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a748a-125">Authorization</span></span>  | <span data-ttu-id="a748a-126">string</span><span class="sxs-lookup"><span data-stu-id="a748a-126">string</span></span>  | <span data-ttu-id="a748a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a748a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a748a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a748a-129">Request body</span></span>
<span data-ttu-id="a748a-130">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a748a-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="a748a-131">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a748a-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="a748a-132">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="a748a-132">Required parameter</span></span> | <span data-ttu-id="a748a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a748a-133">Type</span></span> | <span data-ttu-id="a748a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a748a-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="a748a-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a748a-135">roleTemplateId</span></span> | <span data-ttu-id="a748a-136">string</span><span class="sxs-lookup"><span data-stu-id="a748a-136">string</span></span> | <span data-ttu-id="a748a-p104">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="a748a-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="a748a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a748a-139">Response</span></span>

<span data-ttu-id="a748a-140">В случае успеха этот метод возвратит код отклика `201 Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a748a-140">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a748a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a748a-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a748a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a748a-142">Request</span></span>
<span data-ttu-id="a748a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a748a-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a748a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a748a-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a748a-145">C#</span><span class="sxs-lookup"><span data-stu-id="a748a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a748a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a748a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a748a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a748a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a748a-148">Java</span><span class="sxs-lookup"><span data-stu-id="a748a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a748a-149">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a748a-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a748a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a748a-150">Response</span></span>
<span data-ttu-id="a748a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a748a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


