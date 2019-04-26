---
title: Создание объекта appRoleAssignment
description: Используйте этот API для создания нового Аппролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: cb171e4d6149de5ba169dbf7ad48e87cb055fb47
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335816"
---
# <a name="create-approleassignment"></a><span data-ttu-id="de933-103">Создание объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="de933-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de933-104">Используйте этот API для создания нового Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="de933-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="de933-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de933-105">Permissions</span></span>
<span data-ttu-id="de933-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de933-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de933-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de933-108">Permission type</span></span>      | <span data-ttu-id="de933-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de933-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de933-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de933-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de933-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de933-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de933-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de933-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de933-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de933-113">Not supported.</span></span>    |
|<span data-ttu-id="de933-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de933-114">Application</span></span> | <span data-ttu-id="de933-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de933-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de933-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de933-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="de933-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de933-117">Request headers</span></span>
| <span data-ttu-id="de933-118">Имя</span><span class="sxs-lookup"><span data-stu-id="de933-118">Name</span></span>       | <span data-ttu-id="de933-119">Тип</span><span class="sxs-lookup"><span data-stu-id="de933-119">Type</span></span> | <span data-ttu-id="de933-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de933-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="de933-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de933-121">Authorization</span></span>  | <span data-ttu-id="de933-122">string</span><span class="sxs-lookup"><span data-stu-id="de933-122">string</span></span>  | <span data-ttu-id="de933-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de933-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de933-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de933-125">Request body</span></span>
<span data-ttu-id="de933-126">В тексте запроса добавьте представление объекта [Аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de933-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de933-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="de933-127">Response</span></span>

<span data-ttu-id="de933-128">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de933-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de933-129">Пример</span><span class="sxs-lookup"><span data-stu-id="de933-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de933-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="de933-130">Request</span></span>
<span data-ttu-id="de933-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de933-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="de933-132">В тексте запроса добавьте представление объекта [Аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de933-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="de933-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="de933-133">Response</span></span>
<span data-ttu-id="de933-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de933-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
