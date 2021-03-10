---
title: Удаление объекта directoryObject
description: Удаление directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e47bb98a5445bc8c1a72557ec5affad7e058647b
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625797"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="af408-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="af408-103">Delete directoryObject</span></span>

<span data-ttu-id="af408-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af408-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af408-105">Удаление directoryObject.</span><span class="sxs-lookup"><span data-stu-id="af408-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="af408-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af408-106">Permissions</span></span>
<span data-ttu-id="af408-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="af408-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af408-109">Permission type</span></span>      | <span data-ttu-id="af408-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af408-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af408-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af408-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af408-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af408-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af408-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af408-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af408-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af408-114">Not supported.</span></span>    |
|<span data-ttu-id="af408-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af408-115">Application</span></span> | <span data-ttu-id="af408-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af408-116">Not supported.</span></span> |

<span data-ttu-id="af408-117">**ПРИМЕЧАНИЕ:** Пользователи, группы и контакты — это типы объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="af408-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="af408-118">В результате, если требуется удалить пользователей, можно и нужно использовать следующее разрешение: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af408-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="af408-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af408-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="af408-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af408-120">Request headers</span></span>
| <span data-ttu-id="af408-121">Имя</span><span class="sxs-lookup"><span data-stu-id="af408-121">Name</span></span>       | <span data-ttu-id="af408-122">Тип</span><span class="sxs-lookup"><span data-stu-id="af408-122">Type</span></span> | <span data-ttu-id="af408-123">Описание</span><span class="sxs-lookup"><span data-stu-id="af408-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af408-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="af408-124">Authorization</span></span>  | <span data-ttu-id="af408-125">string</span><span class="sxs-lookup"><span data-stu-id="af408-125">string</span></span>  | <span data-ttu-id="af408-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af408-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af408-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af408-128">Request body</span></span>
<span data-ttu-id="af408-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af408-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af408-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="af408-130">Response</span></span>

<span data-ttu-id="af408-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="af408-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af408-133">Пример</span><span class="sxs-lookup"><span data-stu-id="af408-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af408-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="af408-134">Request</span></span>
<span data-ttu-id="af408-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af408-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="af408-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="af408-136">Response</span></span>
<span data-ttu-id="af408-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af408-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


