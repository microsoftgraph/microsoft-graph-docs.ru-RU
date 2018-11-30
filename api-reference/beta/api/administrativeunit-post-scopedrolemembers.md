---
title: Добавление scopedRoleMember
description: 'Добавьте новый scopedRoleMembership. Примечание: Только роли *пользователя учетной записи администратора* и *администратору службы поддержки* в настоящее время поддерживаются областью действия ролями.'
ms.openlocfilehash: bab8b1ba5d9093617f1aafb48d84f41badef2566
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075742"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="5f922-104">Добавление scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="5f922-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="5f922-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f922-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f922-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f922-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f922-107">Добавьте новый [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="5f922-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="5f922-108">Примечание: Только роли *пользователя учетной записи администратора* и *администратору службы поддержки* в настоящее время поддерживаются областью действия ролями.</span><span class="sxs-lookup"><span data-stu-id="5f922-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f922-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f922-109">Permissions</span></span>
<span data-ttu-id="5f922-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f922-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5f922-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f922-112">Permission type</span></span>      | <span data-ttu-id="5f922-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f922-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f922-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f922-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f922-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f922-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f922-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f922-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f922-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f922-117">Not supported.</span></span>    |
|<span data-ttu-id="5f922-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f922-118">Application</span></span> | <span data-ttu-id="5f922-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f922-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f922-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f922-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="5f922-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f922-121">Request headers</span></span>
| <span data-ttu-id="5f922-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5f922-122">Name</span></span>      |<span data-ttu-id="5f922-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5f922-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f922-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f922-124">Authorization</span></span>  | <span data-ttu-id="5f922-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f922-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f922-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f922-127">Request body</span></span>
<span data-ttu-id="5f922-128">В тексте запроса укажите представление JSON объекта [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5f922-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f922-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f922-129">Response</span></span>

<span data-ttu-id="5f922-130">Успешно завершена, этот метод возвращает `201 Created` объект [scopedRoleMembership](../resources/scopedrolemembership.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5f922-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f922-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5f922-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f922-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f922-132">Request</span></span>
<span data-ttu-id="5f922-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f922-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
<span data-ttu-id="5f922-134">В тексте запроса укажите представление JSON объекта [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5f922-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5f922-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f922-135">Response</span></span>
<span data-ttu-id="5f922-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5f922-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->