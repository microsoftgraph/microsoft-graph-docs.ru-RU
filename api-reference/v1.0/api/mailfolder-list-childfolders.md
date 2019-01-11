---
title: Список childFolders
description: 'Получите коллекцию папок в указанной папке. Можно использовать `.../me/MailFolders` ярлык для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 1d1a002bef6d1e16c48cc484211abe752e4adbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819917"
---
# <a name="list-childfolders"></a><span data-ttu-id="35718-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="35718-104">List childFolders</span></span>

<span data-ttu-id="35718-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="35718-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="35718-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35718-107">Permissions</span></span>
<span data-ttu-id="35718-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35718-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35718-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35718-110">Permission type</span></span>      | <span data-ttu-id="35718-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35718-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35718-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35718-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35718-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35718-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35718-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35718-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35718-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35718-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35718-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35718-116">Application</span></span> | <span data-ttu-id="35718-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35718-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35718-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35718-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35718-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35718-119">Optional query parameters</span></span>
<span data-ttu-id="35718-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35718-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35718-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35718-121">Request headers</span></span>
| <span data-ttu-id="35718-122">Имя</span><span class="sxs-lookup"><span data-stu-id="35718-122">Name</span></span>       | <span data-ttu-id="35718-123">Тип</span><span class="sxs-lookup"><span data-stu-id="35718-123">Type</span></span> | <span data-ttu-id="35718-124">Описание</span><span class="sxs-lookup"><span data-stu-id="35718-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35718-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="35718-125">Authorization</span></span>  | <span data-ttu-id="35718-126">string</span><span class="sxs-lookup"><span data-stu-id="35718-126">string</span></span>  | <span data-ttu-id="35718-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35718-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35718-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35718-129">Request body</span></span>
<span data-ttu-id="35718-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35718-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35718-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="35718-131">Response</span></span>

<span data-ttu-id="35718-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35718-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35718-133">Пример</span><span class="sxs-lookup"><span data-stu-id="35718-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35718-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="35718-134">Request</span></span>
<span data-ttu-id="35718-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35718-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="35718-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="35718-136">Response</span></span>
<span data-ttu-id="35718-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35718-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
