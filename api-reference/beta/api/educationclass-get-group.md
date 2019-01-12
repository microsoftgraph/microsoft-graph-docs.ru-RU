---
title: Получение группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e925775468d13d56e303302b69bb290f5745dcfe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935551"
---
# <a name="get-group"></a><span data-ttu-id="ded23-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="ded23-103">Get group</span></span>

> <span data-ttu-id="ded23-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ded23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ded23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ded23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ded23-106">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="ded23-106">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="ded23-107">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="ded23-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="ded23-108">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="ded23-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="ded23-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ded23-109">Permissions</span></span>
<span data-ttu-id="ded23-110">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="ded23-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="ded23-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ded23-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ded23-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ded23-112">Permission type</span></span>      | <span data-ttu-id="ded23-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ded23-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ded23-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ded23-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="ded23-115">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ded23-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="ded23-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ded23-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ded23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ded23-117">Not supported.</span></span>  |
|<span data-ttu-id="ded23-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ded23-118">Application</span></span> | <span data-ttu-id="ded23-119">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ded23-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="ded23-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ded23-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="ded23-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ded23-121">Request headers</span></span>
| <span data-ttu-id="ded23-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ded23-122">Header</span></span>       | <span data-ttu-id="ded23-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ded23-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ded23-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ded23-124">Authorization</span></span>  | <span data-ttu-id="ded23-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ded23-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ded23-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ded23-127">Request body</span></span>
<span data-ttu-id="ded23-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ded23-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ded23-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ded23-129">Response</span></span>
<span data-ttu-id="ded23-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ded23-130">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ded23-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ded23-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ded23-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ded23-132">Request</span></span>
<span data-ttu-id="ded23-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ded23-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="ded23-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ded23-134">Response</span></span>
<span data-ttu-id="ded23-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ded23-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ded23-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ded23-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
