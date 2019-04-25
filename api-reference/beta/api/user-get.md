---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b0a05ee2e2bd2b4f5d2e66f5c2e0efcf27efb59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536476"
---
# <a name="get-a-user"></a><span data-ttu-id="ebf6a-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="ebf6a-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf6a-104">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="ebf6a-105">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebf6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebf6a-106">Permissions</span></span>
<span data-ttu-id="ebf6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebf6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebf6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebf6a-109">Permission type</span></span>      | <span data-ttu-id="ebf6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebf6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebf6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebf6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebf6a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebf6a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ebf6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebf6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebf6a-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebf6a-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="ebf6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebf6a-115">Application</span></span> | <span data-ttu-id="ebf6a-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6a-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebf6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebf6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebf6a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebf6a-118">Optional query parameters</span></span>
<span data-ttu-id="ebf6a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ebf6a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebf6a-120">Request headers</span></span>
| <span data-ttu-id="ebf6a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebf6a-121">Header</span></span>       | <span data-ttu-id="ebf6a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ebf6a-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ebf6a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebf6a-123">Authorization</span></span>  | <span data-ttu-id="ebf6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ebf6a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebf6a-126">Content-Type</span></span>   | <span data-ttu-id="ebf6a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ebf6a-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebf6a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebf6a-128">Request body</span></span>
<span data-ttu-id="ebf6a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebf6a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebf6a-130">Response</span></span>

<span data-ttu-id="ebf6a-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebf6a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ebf6a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebf6a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebf6a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="ebf6a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebf6a-134">Response</span></span>
<span data-ttu-id="ebf6a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-135">Here is an example of the response.</span></span> <span data-ttu-id="ebf6a-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ebf6a-136">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
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

## <a name="see-also"></a><span data-ttu-id="ebf6a-137">См. также</span><span class="sxs-lookup"><span data-stu-id="ebf6a-137">See also</span></span>

- [<span data-ttu-id="ebf6a-138">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ebf6a-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ebf6a-139">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ebf6a-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ebf6a-140">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ebf6a-140">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
