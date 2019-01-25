---
title: Создание privilegedApproval
description: Используйте этот интерфейс API для создания нового privilegedApproval.
localization_priority: Normal
ms.openlocfilehash: 076184417f6dc77dfc57046d75a3274716232f3b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507679"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="9439b-103">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9439b-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9439b-104">Используйте этот интерфейс API для создания нового privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="9439b-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="9439b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9439b-105">Permissions</span></span>
<span data-ttu-id="9439b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9439b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9439b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9439b-108">Permission type</span></span>      | <span data-ttu-id="9439b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9439b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9439b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9439b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9439b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9439b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9439b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9439b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9439b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9439b-113">Not supported.</span></span>    |
|<span data-ttu-id="9439b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9439b-114">Application</span></span> | <span data-ttu-id="9439b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9439b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9439b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9439b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="9439b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9439b-117">Request headers</span></span>
| <span data-ttu-id="9439b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9439b-118">Name</span></span>       | <span data-ttu-id="9439b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9439b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9439b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9439b-120">Authorization</span></span>  | <span data-ttu-id="9439b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9439b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9439b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9439b-123">Request body</span></span>
<span data-ttu-id="9439b-124">В тексте запроса укажите представление JSON объекта [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="9439b-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9439b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="9439b-125">Response</span></span>

<span data-ttu-id="9439b-126">Успешно завершена, этот метод возвращает `201 Created` объект [privilegedApproval](../resources/privilegedapproval.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9439b-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="9439b-127">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="9439b-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9439b-128">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="9439b-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="9439b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9439b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9439b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9439b-130">Request</span></span>
<span data-ttu-id="9439b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9439b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="9439b-132">В тексте запроса укажите представление JSON объекта [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="9439b-132">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9439b-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9439b-133">Response</span></span>
<span data-ttu-id="9439b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9439b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

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
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
