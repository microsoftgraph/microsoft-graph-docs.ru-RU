---
title: Удаление объекта directoryObject
description: Удалите directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: e291004f13eaf6d0f24750002c8068d3e97b3052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865206"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="ba8d0-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ba8d0-103">Delete directoryObject</span></span>

> <span data-ttu-id="ba8d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba8d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba8d0-106">Удалите directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba8d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8d0-107">Permissions</span></span>
<span data-ttu-id="ba8d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba8d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ba8d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8d0-110">Permission type</span></span>      | <span data-ttu-id="ba8d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba8d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba8d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba8d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba8d0-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba8d0-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba8d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba8d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba8d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-115">Not supported.</span></span>    |
|<span data-ttu-id="ba8d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba8d0-116">Application</span></span> | <span data-ttu-id="ba8d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-117">Not supported.</span></span> |

<span data-ttu-id="ba8d0-118">**Примечание:** Пользователей, групп и контакты, типы объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="ba8d0-119">В результате, если вам потребуется удалить пользователей, следующие разрешения можно и должен использоваться: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8d0-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="ba8d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba8d0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ba8d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba8d0-121">Request headers</span></span>
| <span data-ttu-id="ba8d0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ba8d0-122">Name</span></span>       | <span data-ttu-id="ba8d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ba8d0-123">Type</span></span> | <span data-ttu-id="ba8d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ba8d0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba8d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8d0-125">Authorization</span></span>  | <span data-ttu-id="ba8d0-126">string</span><span class="sxs-lookup"><span data-stu-id="ba8d0-126">string</span></span>  | <span data-ttu-id="ba8d0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba8d0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba8d0-129">Request body</span></span>
<span data-ttu-id="ba8d0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba8d0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8d0-131">Response</span></span>

<span data-ttu-id="ba8d0-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba8d0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ba8d0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba8d0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba8d0-135">Request</span></span>
<span data-ttu-id="ba8d0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="ba8d0-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba8d0-137">Response</span></span>
<span data-ttu-id="ba8d0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba8d0-138">Here is an example of the response.</span></span> 
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
