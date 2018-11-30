---
title: Удаление фотографии
description: Удаление фотографии.
ms.openlocfilehash: 3a227ceb503caf947786adfb35265755e6059b0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079824"
---
# <a name="delete-photo"></a><span data-ttu-id="0ae72-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="0ae72-103">Delete photo</span></span>

> <span data-ttu-id="0ae72-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ae72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ae72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ae72-106">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="0ae72-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ae72-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae72-107">Permissions</span></span>
<span data-ttu-id="0ae72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae72-110">Permission type</span></span>      | <span data-ttu-id="0ae72-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ae72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ae72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ae72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ae72-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ae72-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ae72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ae72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ae72-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ae72-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ae72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ae72-116">Application</span></span> | <span data-ttu-id="0ae72-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae72-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ae72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ae72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="0ae72-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ae72-119">Request headers</span></span>
| <span data-ttu-id="0ae72-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ae72-120">Name</span></span>       | <span data-ttu-id="0ae72-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0ae72-121">Type</span></span> | <span data-ttu-id="0ae72-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0ae72-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ae72-123">if-match</span><span class="sxs-lookup"><span data-stu-id="0ae72-123">if-match</span></span>  | <span data-ttu-id="0ae72-124">string</span><span class="sxs-lookup"><span data-stu-id="0ae72-124">string</span></span>  | <span data-ttu-id="0ae72-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="0ae72-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="0ae72-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ae72-126">Authorization</span></span>  | <span data-ttu-id="0ae72-127">string</span><span class="sxs-lookup"><span data-stu-id="0ae72-127">string</span></span>  | <span data-ttu-id="0ae72-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ae72-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ae72-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ae72-130">Request body</span></span>
<span data-ttu-id="0ae72-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ae72-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ae72-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae72-132">Response</span></span>

<span data-ttu-id="0ae72-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0ae72-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae72-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0ae72-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ae72-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ae72-136">Request</span></span>
<span data-ttu-id="0ae72-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ae72-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="0ae72-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ae72-138">Response</span></span>
<span data-ttu-id="0ae72-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ae72-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
