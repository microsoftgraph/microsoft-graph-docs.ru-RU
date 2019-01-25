---
title: 'privilegedRoleAssignment: Мой'
description: Получение назначения ролей привилегированной инициатора.
localization_priority: Normal
ms.openlocfilehash: fe3f0486d7c5f011abbac60deed831b798802aef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520062"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="4195c-103">privilegedRoleAssignment: Мой</span><span class="sxs-lookup"><span data-stu-id="4195c-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4195c-104">Получение назначения ролей привилегированной инициатора.</span><span class="sxs-lookup"><span data-stu-id="4195c-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="4195c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4195c-105">Permissions</span></span>
<span data-ttu-id="4195c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4195c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4195c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4195c-108">Permission type</span></span>      | <span data-ttu-id="4195c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4195c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4195c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4195c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4195c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4195c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4195c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4195c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4195c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4195c-113">Not supported.</span></span>    |
|<span data-ttu-id="4195c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4195c-114">Application</span></span> | <span data-ttu-id="4195c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4195c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4195c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4195c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="4195c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4195c-117">Request headers</span></span>
| <span data-ttu-id="4195c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4195c-118">Name</span></span>       | <span data-ttu-id="4195c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4195c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4195c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4195c-120">Authorization</span></span>  | <span data-ttu-id="4195c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4195c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4195c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4195c-123">Request body</span></span>
<span data-ttu-id="4195c-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4195c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4195c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4195c-125">Response</span></span>

<span data-ttu-id="4195c-126">Успешно завершена, этот метод возвращает `200 OK` кода и [privilegedRoleAssignment](../resources/privilegedroleassignment.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4195c-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4195c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4195c-127">Example</span></span>
<span data-ttu-id="4195c-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4195c-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4195c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4195c-129">Request</span></span>
<span data-ttu-id="4195c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4195c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="4195c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4195c-131">Response</span></span>
<span data-ttu-id="4195c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4195c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
