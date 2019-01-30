---
title: Добавление scopedRoleMember
description: 'Добавьте новый scopedRoleMembership. Примечание: Только роли *пользователя учетной записи администратора* и *администратору службы поддержки* в настоящее время поддерживаются областью действия ролями.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f94c66bd804d2771987ee58539abdbe073abc03
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640359"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="8c025-104">Добавление scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="8c025-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c025-105">Добавьте новый [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="8c025-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="8c025-106">Примечание: Только роли *пользователя учетной записи администратора* и *администратору службы поддержки* в настоящее время поддерживаются областью действия ролями.</span><span class="sxs-lookup"><span data-stu-id="8c025-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c025-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c025-107">Permissions</span></span>
<span data-ttu-id="8c025-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c025-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c025-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c025-110">Permission type</span></span>      | <span data-ttu-id="8c025-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c025-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c025-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c025-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c025-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c025-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c025-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c025-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c025-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c025-115">Not supported.</span></span>    |
|<span data-ttu-id="8c025-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c025-116">Application</span></span> | <span data-ttu-id="8c025-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c025-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c025-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c025-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="8c025-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c025-119">Request headers</span></span>
| <span data-ttu-id="8c025-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8c025-120">Name</span></span>      |<span data-ttu-id="8c025-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8c025-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c025-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c025-122">Authorization</span></span>  | <span data-ttu-id="8c025-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c025-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c025-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c025-125">Request body</span></span>
<span data-ttu-id="8c025-126">В тексте запроса укажите представление JSON объекта [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="8c025-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8c025-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c025-127">Response</span></span>

<span data-ttu-id="8c025-128">Успешно завершена, этот метод возвращает `201 Created` объект [scopedRoleMembership](../resources/scopedrolemembership.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8c025-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c025-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8c025-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c025-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c025-130">Request</span></span>
<span data-ttu-id="8c025-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c025-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="8c025-132">В тексте запроса укажите представление JSON объекта [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="8c025-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8c025-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c025-133">Response</span></span>
<span data-ttu-id="8c025-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c025-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
