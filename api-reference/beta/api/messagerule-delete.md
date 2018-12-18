---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
ms.openlocfilehash: e10cebf6b2758a21a8bf70e505edcebb7f27082c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305378"
---
# <a name="delete-messagerule"></a><span data-ttu-id="b5f9c-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="b5f9c-103">Delete messageRule</span></span>

> <span data-ttu-id="b5f9c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5f9c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5f9c-106">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="b5f9c-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5f9c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f9c-107">Permissions</span></span>
<span data-ttu-id="b5f9c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5f9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f9c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f9c-110">Permission type</span></span>      | <span data-ttu-id="b5f9c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5f9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5f9c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5f9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5f9c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f9c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b5f9c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5f9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f9c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f9c-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b5f9c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5f9c-116">Application</span></span> | <span data-ttu-id="b5f9c-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f9c-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5f9c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5f9c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5f9c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5f9c-119">Request headers</span></span>
| <span data-ttu-id="b5f9c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b5f9c-120">Name</span></span>       | <span data-ttu-id="b5f9c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f9c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5f9c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5f9c-122">Authorization</span></span>  | <span data-ttu-id="b5f9c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b5f9c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5f9c-125">Request body</span></span>
<span data-ttu-id="b5f9c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b5f9c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f9c-127">Response</span></span>
<span data-ttu-id="b5f9c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f9c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b5f9c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5f9c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5f9c-131">Request</span></span>
<span data-ttu-id="b5f9c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="b5f9c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5f9c-133">Response</span></span>
<span data-ttu-id="b5f9c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5f9c-134">Here is an example of the response.</span></span> 
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