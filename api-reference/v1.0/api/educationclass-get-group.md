---
title: Вывод группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5397330872d5317d5b7c4a7e8c6cb0051a23dfb0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271745"
---
# <a name="get-group"></a><span data-ttu-id="ec2f1-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="ec2f1-103">Get group</span></span>

<span data-ttu-id="ec2f1-104">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="ec2f1-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="ec2f1-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec2f1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2f1-107">Permissions</span></span>
<span data-ttu-id="ec2f1-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="ec2f1-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec2f1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec2f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2f1-110">Permission type</span></span>      | <span data-ttu-id="ec2f1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec2f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec2f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec2f1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec2f1-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec2f1-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="ec2f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec2f1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec2f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-115">Not supported.</span></span>  |
|<span data-ttu-id="ec2f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec2f1-116">Application</span></span> | <span data-ttu-id="ec2f1-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec2f1-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="ec2f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec2f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="ec2f1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec2f1-119">Request headers</span></span>
| <span data-ttu-id="ec2f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec2f1-120">Header</span></span>       | <span data-ttu-id="ec2f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec2f1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec2f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec2f1-122">Authorization</span></span>  | <span data-ttu-id="ec2f1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec2f1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec2f1-125">Request body</span></span>
<span data-ttu-id="ec2f1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec2f1-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec2f1-127">Response</span></span>
<span data-ttu-id="ec2f1-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec2f1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ec2f1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec2f1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec2f1-130">Request</span></span>
<span data-ttu-id="ec2f1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="ec2f1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec2f1-132">Response</span></span>
<span data-ttu-id="ec2f1-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ec2f1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec2f1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ec2f1-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ec2f1-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ec2f1-137">C#</span><span class="sxs-lookup"><span data-stu-id="ec2f1-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec2f1-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec2f1-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ec2f1-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ec2f1-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-get-group.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-get-group.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-get-group.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
