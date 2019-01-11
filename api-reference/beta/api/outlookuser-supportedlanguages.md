---
title: 'outlookUser: supportedLanguages'
description: Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.
localization_priority: Normal
ms.openlocfilehash: 8d3a830a34d4b6d59bae1a601562ab6d70f7a39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868581"
---
# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="18e12-103">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="18e12-103">outlookUser: supportedLanguages</span></span>

> <span data-ttu-id="18e12-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18e12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18e12-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18e12-106">Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="18e12-106">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="18e12-107">Настраивая клиент Outlook, пользователь выбирает язык из этого списка.</span><span class="sxs-lookup"><span data-stu-id="18e12-107">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="18e12-108">После этого вы можете получить выбранный язык вместе с [ настройками почтового ящика пользователя](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-108">You can subsequently get the preferred language by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="18e12-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18e12-109">Permissions</span></span>
<span data-ttu-id="18e12-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e12-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e12-112">Permission type</span></span>      | <span data-ttu-id="18e12-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e12-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18e12-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e12-114">Delegated (work or school account)</span></span> | <span data-ttu-id="18e12-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="18e12-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="18e12-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e12-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18e12-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="18e12-117">User.Read</span></span>    |
|<span data-ttu-id="18e12-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18e12-118">Application</span></span> | <span data-ttu-id="18e12-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="18e12-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e12-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e12-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="18e12-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e12-121">Request headers</span></span>
| <span data-ttu-id="18e12-122">Имя</span><span class="sxs-lookup"><span data-stu-id="18e12-122">Name</span></span>       | <span data-ttu-id="18e12-123">Тип</span><span class="sxs-lookup"><span data-stu-id="18e12-123">Type</span></span> | <span data-ttu-id="18e12-124">Описание</span><span class="sxs-lookup"><span data-stu-id="18e12-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18e12-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e12-125">Authorization</span></span>  | <span data-ttu-id="18e12-126">string</span><span class="sxs-lookup"><span data-stu-id="18e12-126">string</span></span>  | <span data-ttu-id="18e12-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18e12-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="18e12-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18e12-129">Request body</span></span>
<span data-ttu-id="18e12-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18e12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18e12-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="18e12-131">Response</span></span>
<span data-ttu-id="18e12-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [localeInfo](../resources/localeinfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="18e12-132">If successful, this method returns `200 OK` response code and a collection of [localeInfo](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18e12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="18e12-133">Example</span></span>
<span data-ttu-id="18e12-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="18e12-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18e12-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e12-135">Request</span></span>
<span data-ttu-id="18e12-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e12-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="18e12-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="18e12-137">Response</span></span>
<span data-ttu-id="18e12-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18e12-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
