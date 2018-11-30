---
title: Удаление servicePrincipal
description: Удалите servicePrincipal.
ms.openlocfilehash: 363c6a17a7181d72214329c3e6f50433d84a1786
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077674"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="e1616-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e1616-103">Delete servicePrincipal</span></span>

> <span data-ttu-id="e1616-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1616-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1616-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1616-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1616-106">Удалите servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="e1616-106">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1616-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1616-107">Permissions</span></span>
<span data-ttu-id="e1616-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1616-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1616-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1616-110">Permission type</span></span>      | <span data-ttu-id="e1616-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1616-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1616-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1616-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1616-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1616-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1616-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1616-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1616-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1616-115">Not supported.</span></span>    |
|<span data-ttu-id="e1616-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e1616-116">Application</span></span> | <span data-ttu-id="e1616-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1616-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1616-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1616-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e1616-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1616-119">Request headers</span></span>
| <span data-ttu-id="e1616-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e1616-120">Name</span></span>       | <span data-ttu-id="e1616-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e1616-121">Type</span></span> | <span data-ttu-id="e1616-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1616-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1616-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1616-123">Authorization</span></span>  | <span data-ttu-id="e1616-124">string</span><span class="sxs-lookup"><span data-stu-id="e1616-124">string</span></span>  | <span data-ttu-id="e1616-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1616-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1616-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1616-127">Request body</span></span>
<span data-ttu-id="e1616-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1616-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1616-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1616-129">Response</span></span>

<span data-ttu-id="e1616-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e1616-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1616-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e1616-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1616-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1616-133">Request</span></span>
<span data-ttu-id="e1616-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1616-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="e1616-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1616-135">Response</span></span>
<span data-ttu-id="e1616-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1616-136">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->