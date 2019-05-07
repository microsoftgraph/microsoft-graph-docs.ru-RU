---
title: 'servicePrincipal: Добавление владельца'
description: Используйте этот API, чтобы добавить владельца для субъекта-службы.
localization_priority: Normal
ms.openlocfilehash: 6da4b2b7b9ae83aae5bd818454047cdb31166484
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638600"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="d9359-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="d9359-103">servicePrincipal: Add owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9359-104">Используйте этот API, чтобы добавить владельца для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="d9359-104">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9359-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9359-105">Permissions</span></span>
<span data-ttu-id="d9359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9359-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9359-108">Permission type</span></span>      | <span data-ttu-id="d9359-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9359-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9359-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9359-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9359-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9359-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9359-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9359-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9359-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9359-113">Not supported.</span></span>    |
|<span data-ttu-id="d9359-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9359-114">Application</span></span> | <span data-ttu-id="d9359-115">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d9359-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9359-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9359-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="d9359-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9359-117">Request headers</span></span>
| <span data-ttu-id="d9359-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9359-118">Name</span></span>       | <span data-ttu-id="d9359-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d9359-119">Type</span></span> | <span data-ttu-id="d9359-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9359-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9359-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9359-121">Authorization</span></span>  | <span data-ttu-id="d9359-122">string</span><span class="sxs-lookup"><span data-stu-id="d9359-122">string</span></span>  | <span data-ttu-id="d9359-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9359-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9359-125">Request body</span></span>
<span data-ttu-id="d9359-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9359-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9359-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9359-127">Response</span></span>

<span data-ttu-id="d9359-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9359-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9359-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d9359-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9359-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9359-130">Request</span></span>
<span data-ttu-id="d9359-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9359-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="d9359-132">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9359-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9359-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9359-133">Response</span></span>
<span data-ttu-id="d9359-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9359-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d9359-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d9359-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9359-138">Язык</span><span class="sxs-lookup"><span data-stu-id="d9359-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
