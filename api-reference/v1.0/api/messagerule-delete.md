---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 570970296444b5bb4d5033bf26a03214d9fa8dac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585218"
---
# <a name="delete-messagerule"></a><span data-ttu-id="ae174-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="ae174-103">Delete messageRule</span></span>


<span data-ttu-id="ae174-104">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="ae174-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae174-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae174-105">Permissions</span></span>
<span data-ttu-id="ae174-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae174-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae174-108">Permission type</span></span>      | <span data-ttu-id="ae174-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae174-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae174-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae174-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae174-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae174-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ae174-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae174-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae174-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae174-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ae174-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae174-114">Application</span></span> | <span data-ttu-id="ae174-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae174-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae174-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae174-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ae174-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae174-117">Request headers</span></span>
| <span data-ttu-id="ae174-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ae174-118">Name</span></span>       | <span data-ttu-id="ae174-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ae174-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae174-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae174-120">Authorization</span></span>  | <span data-ttu-id="ae174-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae174-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ae174-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae174-123">Request body</span></span>
<span data-ttu-id="ae174-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae174-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ae174-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae174-125">Response</span></span>
<span data-ttu-id="ae174-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ae174-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae174-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ae174-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae174-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae174-129">Request</span></span>
<span data-ttu-id="ae174-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae174-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="ae174-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae174-131">Response</span></span>
<span data-ttu-id="ae174-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae174-132">Here is an example of the response.</span></span> 
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
