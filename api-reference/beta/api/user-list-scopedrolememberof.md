---
title: Список Скопедадминистратороф
description: Получение списка Scopedrolemembership изменен для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6d458aa275b7405d25f60c8946e544b79bc7ac2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544213"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="6ecf9-103">Список Скопедадминистратороф</span><span class="sxs-lookup"><span data-stu-id="6ecf9-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ecf9-104">Получение списка [scopedrolemembership изменен](../resources/scopedrolemembership.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ecf9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecf9-105">Permissions</span></span>
<span data-ttu-id="6ecf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ecf9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecf9-108">Permission type</span></span>      | <span data-ttu-id="6ecf9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ecf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ecf9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ecf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ecf9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ecf9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ecf9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ecf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ecf9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-113">Not supported.</span></span>    |
|<span data-ttu-id="6ecf9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ecf9-114">Application</span></span> | <span data-ttu-id="6ecf9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ecf9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ecf9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ecf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ecf9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ecf9-117">Optional query parameters</span></span>
<span data-ttu-id="6ecf9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ecf9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ecf9-119">Request headers</span></span>
| <span data-ttu-id="6ecf9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ecf9-120">Header</span></span>       | <span data-ttu-id="6ecf9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ecf9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ecf9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ecf9-122">Authorization</span></span>  | <span data-ttu-id="6ecf9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ecf9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ecf9-125">Request body</span></span>
<span data-ttu-id="6ecf9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ecf9-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ecf9-127">Response</span></span>

<span data-ttu-id="6ecf9-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ecf9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6ecf9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ecf9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecf9-130">Request</span></span>
<span data-ttu-id="6ecf9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="6ecf9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecf9-132">Response</span></span>
<span data-ttu-id="6ecf9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ecf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
