---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
ms.openlocfilehash: 5fe208b72ddc28ca3d2ee5d2b0f1c48113e49c64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343465"
---
# <a name="delete-messagerule"></a><span data-ttu-id="003db-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="003db-103">Delete messageRule</span></span>


<span data-ttu-id="003db-104">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="003db-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="003db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="003db-105">Permissions</span></span>
<span data-ttu-id="003db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="003db-108">Permission type</span></span>      | <span data-ttu-id="003db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="003db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="003db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="003db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="003db-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003db-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="003db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="003db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="003db-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003db-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="003db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="003db-114">Application</span></span> | <span data-ttu-id="003db-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003db-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="003db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="003db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="003db-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="003db-117">Request headers</span></span>
| <span data-ttu-id="003db-118">Имя</span><span class="sxs-lookup"><span data-stu-id="003db-118">Name</span></span>       | <span data-ttu-id="003db-119">Описание</span><span class="sxs-lookup"><span data-stu-id="003db-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="003db-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="003db-120">Authorization</span></span>  | <span data-ttu-id="003db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="003db-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="003db-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="003db-123">Request body</span></span>
<span data-ttu-id="003db-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="003db-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="003db-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="003db-125">Response</span></span>
<span data-ttu-id="003db-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="003db-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003db-128">Пример</span><span class="sxs-lookup"><span data-stu-id="003db-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="003db-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="003db-129">Request</span></span>
<span data-ttu-id="003db-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="003db-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="003db-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="003db-131">Response</span></span>
<span data-ttu-id="003db-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="003db-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->