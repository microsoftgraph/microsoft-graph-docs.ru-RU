---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 2c303ffda5f9f43273178a6b23c72ee465b569dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842310"
---
# <a name="delete-messagerule"></a><span data-ttu-id="d96a0-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="d96a0-103">Delete messageRule</span></span>


<span data-ttu-id="d96a0-104">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="d96a0-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d96a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d96a0-105">Permissions</span></span>
<span data-ttu-id="d96a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d96a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d96a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d96a0-108">Permission type</span></span>      | <span data-ttu-id="d96a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d96a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d96a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d96a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d96a0-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d96a0-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d96a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d96a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d96a0-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d96a0-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d96a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d96a0-114">Application</span></span> | <span data-ttu-id="d96a0-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d96a0-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d96a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d96a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d96a0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d96a0-117">Request headers</span></span>
| <span data-ttu-id="d96a0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d96a0-118">Name</span></span>       | <span data-ttu-id="d96a0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d96a0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d96a0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d96a0-120">Authorization</span></span>  | <span data-ttu-id="d96a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d96a0-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d96a0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d96a0-123">Request body</span></span>
<span data-ttu-id="d96a0-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d96a0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d96a0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d96a0-125">Response</span></span>
<span data-ttu-id="d96a0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d96a0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d96a0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d96a0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d96a0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d96a0-129">Request</span></span>
<span data-ttu-id="d96a0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d96a0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="d96a0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d96a0-131">Response</span></span>
<span data-ttu-id="d96a0-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d96a0-132">Here is an example of the response.</span></span> 
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
