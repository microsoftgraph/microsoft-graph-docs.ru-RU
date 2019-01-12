---
title: Удаление объекта directoryObject
description: Удалите directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87ecefaac625153407bbc796870e540c3a4e83be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916217"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="d21e9-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="d21e9-103">Delete directoryObject</span></span>

> <span data-ttu-id="d21e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d21e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d21e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d21e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d21e9-106">Удалите directoryObject.</span><span class="sxs-lookup"><span data-stu-id="d21e9-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="d21e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d21e9-107">Permissions</span></span>
<span data-ttu-id="d21e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d21e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d21e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d21e9-110">Permission type</span></span>      | <span data-ttu-id="d21e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d21e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d21e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d21e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d21e9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d21e9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d21e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d21e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d21e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d21e9-115">Not supported.</span></span>    |
|<span data-ttu-id="d21e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d21e9-116">Application</span></span> | <span data-ttu-id="d21e9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d21e9-117">Not supported.</span></span> |

<span data-ttu-id="d21e9-118">**Примечание:** Пользователей, групп и контакты, типы объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="d21e9-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="d21e9-119">В результате, если вам потребуется удалить пользователей, следующие разрешения можно и должен использоваться: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d21e9-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="d21e9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d21e9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d21e9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d21e9-121">Request headers</span></span>
| <span data-ttu-id="d21e9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d21e9-122">Name</span></span>       | <span data-ttu-id="d21e9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d21e9-123">Type</span></span> | <span data-ttu-id="d21e9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d21e9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d21e9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d21e9-125">Authorization</span></span>  | <span data-ttu-id="d21e9-126">string</span><span class="sxs-lookup"><span data-stu-id="d21e9-126">string</span></span>  | <span data-ttu-id="d21e9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d21e9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d21e9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d21e9-129">Request body</span></span>
<span data-ttu-id="d21e9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d21e9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d21e9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d21e9-131">Response</span></span>

<span data-ttu-id="d21e9-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d21e9-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d21e9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d21e9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d21e9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d21e9-135">Request</span></span>
<span data-ttu-id="d21e9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d21e9-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="d21e9-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d21e9-137">Response</span></span>
<span data-ttu-id="d21e9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d21e9-138">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
