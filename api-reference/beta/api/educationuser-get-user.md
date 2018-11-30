---
title: Получение пользователя
description: Получение простого каталога **user**, который соответствует этому объекту **educationUser**.
ms.openlocfilehash: e026fbb1b9294d99e124b16209465c530e229b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080323"
---
# <a name="get-user"></a><span data-ttu-id="8ab3c-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="8ab3c-103">Get user</span></span>

> <span data-ttu-id="8ab3c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ab3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ab3c-106">Получение простого каталога **user**, который соответствует этому объекту **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-106">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="8ab3c-107">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="8ab3c-108">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ab3c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab3c-109">Permissions</span></span>
<span data-ttu-id="8ab3c-110">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="8ab3c-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ab3c-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ab3c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab3c-112">Permission type</span></span>      | <span data-ttu-id="8ab3c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ab3c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ab3c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ab3c-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8ab3c-115">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All или User.Read</span><span class="sxs-lookup"><span data-stu-id="8ab3c-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="8ab3c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ab3c-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8ab3c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-117">Not supported.</span></span>  |
|<span data-ttu-id="8ab3c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ab3c-118">Application</span></span> | <span data-ttu-id="8ab3c-119">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ab3c-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="8ab3c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ab3c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="8ab3c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ab3c-121">Request headers</span></span>
| <span data-ttu-id="8ab3c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ab3c-122">Header</span></span>       | <span data-ttu-id="8ab3c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8ab3c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ab3c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ab3c-124">Authorization</span></span>  | <span data-ttu-id="8ab3c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ab3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ab3c-127">Request body</span></span>
<span data-ttu-id="8ab3c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8ab3c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ab3c-129">Response</span></span>
<span data-ttu-id="8ab3c-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-130">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ab3c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8ab3c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ab3c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ab3c-132">Request</span></span>
<span data-ttu-id="8ab3c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/user
```
##### <a name="response"></a><span data-ttu-id="8ab3c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ab3c-134">Response</span></span>
<span data-ttu-id="8ab3c-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8ab3c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ab3c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->