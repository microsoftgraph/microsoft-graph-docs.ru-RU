---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cfb0f1840ca4a4de0a82b90a4525a8f26b35536d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985566"
---
# <a name="delete-messagerule"></a><span data-ttu-id="5ef43-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="5ef43-103">Delete messageRule</span></span>

> <span data-ttu-id="5ef43-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5ef43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ef43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ef43-106">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="5ef43-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ef43-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ef43-107">Permissions</span></span>
<span data-ttu-id="5ef43-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ef43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ef43-110">Permission type</span></span>      | <span data-ttu-id="5ef43-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ef43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ef43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ef43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ef43-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ef43-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5ef43-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ef43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ef43-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ef43-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5ef43-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ef43-116">Application</span></span> | <span data-ttu-id="5ef43-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ef43-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ef43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ef43-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5ef43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ef43-119">Request headers</span></span>
| <span data-ttu-id="5ef43-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5ef43-120">Name</span></span>       | <span data-ttu-id="5ef43-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5ef43-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ef43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ef43-122">Authorization</span></span>  | <span data-ttu-id="5ef43-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ef43-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5ef43-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ef43-125">Request body</span></span>
<span data-ttu-id="5ef43-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ef43-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5ef43-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ef43-127">Response</span></span>
<span data-ttu-id="5ef43-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5ef43-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ef43-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5ef43-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ef43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ef43-131">Request</span></span>
<span data-ttu-id="5ef43-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ef43-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="5ef43-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ef43-133">Response</span></span>
<span data-ttu-id="5ef43-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ef43-134">Here is an example of the response.</span></span> 
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
