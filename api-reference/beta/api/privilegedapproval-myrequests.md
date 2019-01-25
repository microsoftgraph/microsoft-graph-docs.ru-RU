---
title: 'privilegedApproval: myRequests'
description: Получите запрашивающего запросов на утверждение.
localization_priority: Normal
ms.openlocfilehash: 9fcbdab424c98633a8f543875b9b7c2275894df0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512894"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="c0018-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="c0018-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0018-104">Получите запрашивающего запросов на утверждение.</span><span class="sxs-lookup"><span data-stu-id="c0018-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0018-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0018-105">Permissions</span></span>
<span data-ttu-id="c0018-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0018-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0018-108">Permission type</span></span>      | <span data-ttu-id="c0018-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0018-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0018-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0018-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0018-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0018-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0018-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0018-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0018-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0018-113">Not supported.</span></span>    |
|<span data-ttu-id="c0018-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0018-114">Application</span></span> | <span data-ttu-id="c0018-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0018-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0018-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0018-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="c0018-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0018-117">Request headers</span></span>
| <span data-ttu-id="c0018-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c0018-118">Name</span></span>       | <span data-ttu-id="c0018-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c0018-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0018-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0018-120">Authorization</span></span>  | <span data-ttu-id="c0018-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0018-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0018-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0018-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c0018-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0018-124">Response</span></span>

<span data-ttu-id="c0018-125">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedApproval](../resources/privilegedapproval.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c0018-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="c0018-126">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="c0018-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c0018-127">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c0018-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c0018-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c0018-128">Example</span></span>
<span data-ttu-id="c0018-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c0018-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c0018-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0018-130">Request</span></span>
<span data-ttu-id="c0018-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0018-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="c0018-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0018-132">Response</span></span>
<span data-ttu-id="c0018-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c0018-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
