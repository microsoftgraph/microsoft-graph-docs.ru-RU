---
title: Удаление объекта directoryObject
description: Удалите directoryObject.
author: lleonard-msft
ms.openlocfilehash: f53ffc488529c2af4b566ada52f213d1fc132c60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361413"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="ad7ce-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ad7ce-103">Delete directoryObject</span></span>

> <span data-ttu-id="ad7ce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad7ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad7ce-106">Удалите directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad7ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad7ce-107">Permissions</span></span>
<span data-ttu-id="ad7ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad7ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad7ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad7ce-110">Permission type</span></span>      | <span data-ttu-id="ad7ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad7ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad7ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad7ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad7ce-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad7ce-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad7ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad7ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad7ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-115">Not supported.</span></span>    |
|<span data-ttu-id="ad7ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad7ce-116">Application</span></span> | <span data-ttu-id="ad7ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-117">Not supported.</span></span> |

<span data-ttu-id="ad7ce-118">**Примечание:** Пользователей, групп и контакты, типы объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="ad7ce-119">В результате, если вам потребуется удалить пользователей, следующие разрешения можно и должен использоваться: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad7ce-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="ad7ce-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad7ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ad7ce-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad7ce-121">Request headers</span></span>
| <span data-ttu-id="ad7ce-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ad7ce-122">Name</span></span>       | <span data-ttu-id="ad7ce-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7ce-123">Type</span></span> | <span data-ttu-id="ad7ce-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7ce-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad7ce-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad7ce-125">Authorization</span></span>  | <span data-ttu-id="ad7ce-126">string</span><span class="sxs-lookup"><span data-stu-id="ad7ce-126">string</span></span>  | <span data-ttu-id="ad7ce-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad7ce-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad7ce-129">Request body</span></span>
<span data-ttu-id="ad7ce-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad7ce-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad7ce-131">Response</span></span>

<span data-ttu-id="ad7ce-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad7ce-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ad7ce-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad7ce-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad7ce-135">Request</span></span>
<span data-ttu-id="ad7ce-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="ad7ce-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad7ce-137">Response</span></span>
<span data-ttu-id="ad7ce-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad7ce-138">Here is an example of the response.</span></span> 
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