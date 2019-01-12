---
title: Получение пользователя
description: Получение свойств и связей объекта пользователей.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: da30c60cb9132b70685182fd319f474f9e178720
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914978"
---
# <a name="get-a-user"></a><span data-ttu-id="cebef-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="cebef-103">Get a user</span></span>

> <span data-ttu-id="cebef-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cebef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cebef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cebef-106">Получение свойств и связей объекта пользователей.</span><span class="sxs-lookup"><span data-stu-id="cebef-106">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="cebef-107">Поскольку **пользовательский** ресурс поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **пользователя** .</span><span class="sxs-lookup"><span data-stu-id="cebef-107">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebef-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cebef-108">Permissions</span></span>
<span data-ttu-id="cebef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cebef-111">Permission type</span></span>      | <span data-ttu-id="cebef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cebef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cebef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cebef-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cebef-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cebef-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cebef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cebef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebef-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebef-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="cebef-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cebef-117">Application</span></span> | <span data-ttu-id="cebef-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebef-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cebef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cebef-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cebef-120">Optional query parameters</span></span>
<span data-ttu-id="cebef-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cebef-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cebef-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cebef-122">Request headers</span></span>
| <span data-ttu-id="cebef-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cebef-123">Header</span></span>       | <span data-ttu-id="cebef-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cebef-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cebef-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cebef-125">Authorization</span></span>  | <span data-ttu-id="cebef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cebef-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cebef-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cebef-128">Content-Type</span></span>   | <span data-ttu-id="cebef-129">application/json</span><span class="sxs-lookup"><span data-stu-id="cebef-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cebef-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cebef-130">Request body</span></span>
<span data-ttu-id="cebef-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cebef-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebef-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebef-132">Response</span></span>

<span data-ttu-id="cebef-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cebef-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cebef-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cebef-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cebef-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cebef-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="cebef-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cebef-136">Response</span></span>
<span data-ttu-id="cebef-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cebef-137">Here is an example of the response.</span></span> <span data-ttu-id="cebef-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cebef-138">Note: The response object shown here may be truncated for brevity.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="cebef-139">См. также</span><span class="sxs-lookup"><span data-stu-id="cebef-139">See also</span></span>

- [<span data-ttu-id="cebef-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="cebef-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cebef-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cebef-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cebef-142">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cebef-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
