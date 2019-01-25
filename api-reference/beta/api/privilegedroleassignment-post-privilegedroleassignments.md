---
title: Создание privilegedRoleAssignment
description: Используйте этот интерфейс API для создания нового privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 5522956b129eae8a19fd00b0e70b41380dbdd25e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513405"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="07a2e-103">Создание privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="07a2e-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07a2e-104">Используйте этот интерфейс API для создания нового [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07a2e-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="07a2e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07a2e-105">Permissions</span></span>
<span data-ttu-id="07a2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07a2e-108">Запрашивающая сторона должна иметь роль _Привилегированной роль администратора_ .</span><span class="sxs-lookup"><span data-stu-id="07a2e-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="07a2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07a2e-109">Permission type</span></span>      | <span data-ttu-id="07a2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07a2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07a2e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="07a2e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07a2e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07a2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07a2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07a2e-114">Not supported.</span></span>    |
|<span data-ttu-id="07a2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07a2e-115">Application</span></span> | <span data-ttu-id="07a2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07a2e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07a2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07a2e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="07a2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07a2e-118">Request headers</span></span>
| <span data-ttu-id="07a2e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="07a2e-119">Name</span></span>       | <span data-ttu-id="07a2e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="07a2e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07a2e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07a2e-121">Authorization</span></span>  | <span data-ttu-id="07a2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07a2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07a2e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07a2e-124">Request body</span></span>
<span data-ttu-id="07a2e-125">В тексте запроса укажите представление JSON объекта [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07a2e-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="07a2e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="07a2e-126">Response</span></span>

<span data-ttu-id="07a2e-127">Успешно завершена, этот метод возвращает `201 Created` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07a2e-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="07a2e-128">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="07a2e-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="07a2e-129">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="07a2e-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="07a2e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="07a2e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07a2e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="07a2e-131">Request</span></span>
<span data-ttu-id="07a2e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07a2e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="07a2e-133">В тексте запроса укажите представление JSON объекта [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07a2e-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07a2e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="07a2e-134">Response</span></span>
<span data-ttu-id="07a2e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="07a2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
