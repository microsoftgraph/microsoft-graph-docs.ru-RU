---
title: Удаление orgContact
description: Удалите orgContact.
localization_priority: Normal
ms.openlocfilehash: 3eecd42debf22f7bd2330ddae5a8321b25b7350c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892067"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="3ee84-103">Удаление orgContact</span><span class="sxs-lookup"><span data-stu-id="3ee84-103">Delete orgContact</span></span>

> <span data-ttu-id="3ee84-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ee84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ee84-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee84-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ee84-106">Удалите orgContact.</span><span class="sxs-lookup"><span data-stu-id="3ee84-106">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ee84-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee84-107">Permissions</span></span>
<span data-ttu-id="3ee84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee84-110">Permission type</span></span>      | <span data-ttu-id="3ee84-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ee84-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ee84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ee84-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ee84-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ee84-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ee84-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ee84-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ee84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee84-115">Not supported.</span></span>    |
|<span data-ttu-id="3ee84-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ee84-116">Application</span></span> | <span data-ttu-id="3ee84-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee84-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee84-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ee84-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3ee84-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ee84-119">Request headers</span></span>
| <span data-ttu-id="3ee84-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3ee84-120">Name</span></span>       | <span data-ttu-id="3ee84-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3ee84-121">Type</span></span> | <span data-ttu-id="3ee84-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ee84-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ee84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ee84-123">Authorization</span></span>  | <span data-ttu-id="3ee84-124">string</span><span class="sxs-lookup"><span data-stu-id="3ee84-124">string</span></span>  | <span data-ttu-id="3ee84-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ee84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ee84-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ee84-127">Request body</span></span>
<span data-ttu-id="3ee84-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ee84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee84-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ee84-129">Response</span></span>

<span data-ttu-id="3ee84-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3ee84-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ee84-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3ee84-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ee84-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ee84-133">Request</span></span>
<span data-ttu-id="3ee84-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ee84-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="3ee84-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ee84-135">Response</span></span>
<span data-ttu-id="3ee84-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ee84-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
