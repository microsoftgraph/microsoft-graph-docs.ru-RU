---
title: Вывод группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c02f2c74bb1338e651125bba411a200757313e73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426873"
---
# <a name="get-group"></a><span data-ttu-id="93e3d-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="93e3d-103">Get group</span></span>

<span data-ttu-id="93e3d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e3d-105">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="93e3d-105">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="93e3d-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="93e3d-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="93e3d-107">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="93e3d-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="93e3d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93e3d-108">Permissions</span></span>
<span data-ttu-id="93e3d-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="93e3d-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="93e3d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e3d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e3d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e3d-111">Permission type</span></span>      | <span data-ttu-id="93e3d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e3d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93e3d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e3d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="93e3d-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="93e3d-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="93e3d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e3d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93e3d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e3d-116">Not supported.</span></span>  |
|<span data-ttu-id="93e3d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e3d-117">Application</span></span> | <span data-ttu-id="93e3d-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="93e3d-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="93e3d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e3d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="93e3d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e3d-120">Request headers</span></span>
| <span data-ttu-id="93e3d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93e3d-121">Header</span></span>       | <span data-ttu-id="93e3d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93e3d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93e3d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93e3d-123">Authorization</span></span>  | <span data-ttu-id="93e3d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93e3d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93e3d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93e3d-126">Request body</span></span>
<span data-ttu-id="93e3d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93e3d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93e3d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e3d-128">Response</span></span>
<span data-ttu-id="93e3d-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93e3d-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93e3d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="93e3d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93e3d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e3d-131">Request</span></span>
<span data-ttu-id="93e3d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e3d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93e3d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="93e3d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
# <a name="c"></a>[<span data-ttu-id="93e3d-134">C#</span><span class="sxs-lookup"><span data-stu-id="93e3d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93e3d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93e3d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93e3d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93e3d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93e3d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e3d-137">Response</span></span>
<span data-ttu-id="93e3d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93e3d-138">The following is an example of the response.</span></span> 

><span data-ttu-id="93e3d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93e3d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
