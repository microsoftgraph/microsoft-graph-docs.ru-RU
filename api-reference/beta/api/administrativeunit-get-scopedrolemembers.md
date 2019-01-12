---
title: Получение scopedRoleMember
description: Получение определенных scopedRoleMembership ресурсов.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf707c4bca33302286ab686cf74d9faba63fac7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971706"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="f65a8-103">Получение scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="f65a8-103">Get a scopedRoleMember</span></span>

> <span data-ttu-id="f65a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f65a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f65a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f65a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f65a8-106">Получение определенных [scopedRoleMembership](../resources/scopedrolemembership.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f65a8-106">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="f65a8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f65a8-107">Permissions</span></span>
<span data-ttu-id="f65a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f65a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f65a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f65a8-110">Permission type</span></span>      | <span data-ttu-id="f65a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f65a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f65a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f65a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f65a8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f65a8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f65a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f65a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f65a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f65a8-115">Not supported.</span></span>    |
|<span data-ttu-id="f65a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f65a8-116">Application</span></span> | <span data-ttu-id="f65a8-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f65a8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f65a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f65a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f65a8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f65a8-119">Optional query parameters</span></span>
<span data-ttu-id="f65a8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f65a8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f65a8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f65a8-121">Request headers</span></span>
| <span data-ttu-id="f65a8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f65a8-122">Name</span></span>      |<span data-ttu-id="f65a8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f65a8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f65a8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f65a8-124">Authorization</span></span>  | <span data-ttu-id="f65a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f65a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f65a8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f65a8-127">Request body</span></span>
<span data-ttu-id="f65a8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f65a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f65a8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f65a8-129">Response</span></span>

<span data-ttu-id="f65a8-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект запрошенный [scopedRoleMembership](../resources/scopedrolemembership.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f65a8-130">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f65a8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f65a8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f65a8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f65a8-132">Request</span></span>
<span data-ttu-id="f65a8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f65a8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="f65a8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f65a8-134">Response</span></span>
<span data-ttu-id="f65a8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f65a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
