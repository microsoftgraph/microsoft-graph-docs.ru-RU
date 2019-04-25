---
title: 'Привилежедролеассигнмент: My'
description: Получение привилегированных назначений ролей запрашивающей стороны.
localization_priority: Normal
ms.openlocfilehash: fe3f0486d7c5f011abbac60deed831b798802aef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546560"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="7f76a-103">Привилежедролеассигнмент: My</span><span class="sxs-lookup"><span data-stu-id="7f76a-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f76a-104">Получение привилегированных назначений ролей запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="7f76a-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f76a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f76a-105">Permissions</span></span>
<span data-ttu-id="7f76a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f76a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f76a-108">Permission type</span></span>      | <span data-ttu-id="7f76a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f76a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f76a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f76a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f76a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f76a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f76a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f76a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f76a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f76a-113">Not supported.</span></span>    |
|<span data-ttu-id="7f76a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f76a-114">Application</span></span> | <span data-ttu-id="7f76a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f76a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f76a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f76a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="7f76a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f76a-117">Request headers</span></span>
| <span data-ttu-id="7f76a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7f76a-118">Name</span></span>       | <span data-ttu-id="7f76a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7f76a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f76a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f76a-120">Authorization</span></span>  | <span data-ttu-id="7f76a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f76a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f76a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f76a-123">Request body</span></span>
<span data-ttu-id="7f76a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f76a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f76a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f76a-125">Response</span></span>

<span data-ttu-id="7f76a-126">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f76a-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f76a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7f76a-127">Example</span></span>
<span data-ttu-id="7f76a-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7f76a-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7f76a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f76a-129">Request</span></span>
<span data-ttu-id="7f76a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f76a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="7f76a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f76a-131">Response</span></span>
<span data-ttu-id="7f76a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f76a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
