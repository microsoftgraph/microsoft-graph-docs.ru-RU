---
title: 'privilegedRole: selfDeactivate'
description: Отключение роли, назначенной для инициатора запроса.
localization_priority: Normal
ms.openlocfilehash: 7175af64e7e36087bd048cd6e160393e2bf6377e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528692"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="48bda-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="48bda-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48bda-104">Отключение роли, назначенной для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="48bda-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="48bda-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48bda-105">Permissions</span></span>
<span data-ttu-id="48bda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48bda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="48bda-108">Запрашивающая сторона может вызывать только ```selfDeactivate``` для роли, назначенные ему.</span><span class="sxs-lookup"><span data-stu-id="48bda-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="48bda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48bda-109">Permission type</span></span>      | <span data-ttu-id="48bda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48bda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48bda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48bda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="48bda-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48bda-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48bda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48bda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48bda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bda-114">Not supported.</span></span>    |
|<span data-ttu-id="48bda-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48bda-115">Application</span></span> | <span data-ttu-id="48bda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bda-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48bda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48bda-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="48bda-118">Обратите внимание, что ``<id>`` — это идентификатор целевого роли.</span><span class="sxs-lookup"><span data-stu-id="48bda-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="48bda-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48bda-119">Request headers</span></span>
| <span data-ttu-id="48bda-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48bda-120">Name</span></span>       | <span data-ttu-id="48bda-121">Описание</span><span class="sxs-lookup"><span data-stu-id="48bda-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48bda-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48bda-122">Authorization</span></span>  | <span data-ttu-id="48bda-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48bda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48bda-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48bda-125">Request body</span></span>
<span data-ttu-id="48bda-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48bda-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48bda-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="48bda-127">Response</span></span>

<span data-ttu-id="48bda-128">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48bda-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="48bda-129">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="48bda-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="48bda-130">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="48bda-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="48bda-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48bda-131">Example</span></span>
<span data-ttu-id="48bda-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="48bda-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48bda-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48bda-133">Request</span></span>
<span data-ttu-id="48bda-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48bda-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="48bda-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="48bda-135">Response</span></span>
<span data-ttu-id="48bda-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="48bda-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
