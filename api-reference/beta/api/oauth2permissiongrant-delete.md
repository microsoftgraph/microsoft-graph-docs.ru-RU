---
title: Удаление oAuth2PermissionGrant
description: Удалите oAuth2PermissionGrant.
ms.openlocfilehash: 505a7a58f4c343bd15fd3e1fddce4c07e1d3ef07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081957"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="667d1-103">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="667d1-103">Delete oAuth2PermissionGrant</span></span>

> <span data-ttu-id="667d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="667d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="667d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="667d1-106">Удалите oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="667d1-106">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="667d1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="667d1-107">Permissions</span></span>
<span data-ttu-id="667d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="667d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667d1-110">Permission type</span></span>      | <span data-ttu-id="667d1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="667d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="667d1-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="667d1-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="667d1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667d1-115">Not supported.</span></span>    |
|<span data-ttu-id="667d1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="667d1-116">Application</span></span> | <span data-ttu-id="667d1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667d1-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="667d1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="667d1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="667d1-119">Request headers</span></span>
| <span data-ttu-id="667d1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="667d1-120">Name</span></span>       | <span data-ttu-id="667d1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="667d1-121">Type</span></span> | <span data-ttu-id="667d1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="667d1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="667d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="667d1-123">Authorization</span></span>  | <span data-ttu-id="667d1-124">string</span><span class="sxs-lookup"><span data-stu-id="667d1-124">string</span></span>  | <span data-ttu-id="667d1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="667d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="667d1-127">Request body</span></span>
<span data-ttu-id="667d1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="667d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="667d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="667d1-129">Response</span></span>

<span data-ttu-id="667d1-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="667d1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667d1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="667d1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="667d1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="667d1-133">Request</span></span>
<span data-ttu-id="667d1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667d1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="667d1-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="667d1-135">Response</span></span>
<span data-ttu-id="667d1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="667d1-136">Here is an example of the response.</span></span> 
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
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->