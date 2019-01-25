---
title: Удаление scopedRoleMember
description: Удалите члена группы областью действия роли из единице администрирования.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d373f9f88a6fba2f542abf8f58b751d05f3e75ae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515162"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="7232b-103">Удаление scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="7232b-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7232b-104">Удалите члена группы областью действия роли из единице администрирования.</span><span class="sxs-lookup"><span data-stu-id="7232b-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="7232b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7232b-105">Permissions</span></span>
<span data-ttu-id="7232b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7232b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7232b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7232b-108">Permission type</span></span>      | <span data-ttu-id="7232b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7232b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7232b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7232b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7232b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7232b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7232b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7232b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7232b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7232b-113">Not supported.</span></span>    |
|<span data-ttu-id="7232b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7232b-114">Application</span></span> | <span data-ttu-id="7232b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7232b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7232b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7232b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7232b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7232b-117">Request headers</span></span>
| <span data-ttu-id="7232b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7232b-118">Name</span></span>       | <span data-ttu-id="7232b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7232b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7232b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7232b-120">Authorization</span></span>  | <span data-ttu-id="7232b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7232b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7232b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7232b-123">Request body</span></span>
<span data-ttu-id="7232b-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7232b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7232b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7232b-125">Response</span></span>

<span data-ttu-id="7232b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7232b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7232b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7232b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7232b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7232b-129">Request</span></span>
<span data-ttu-id="7232b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7232b-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="7232b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7232b-131">Response</span></span>
<span data-ttu-id="7232b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7232b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
