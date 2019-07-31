---
title: Удаление объекта directoryObject
description: Удаление directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d3bef033cdd609982f7edf6c178d9393b06dd0a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951178"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="08ab7-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="08ab7-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ab7-104">Удаление directoryObject.</span><span class="sxs-lookup"><span data-stu-id="08ab7-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="08ab7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08ab7-105">Permissions</span></span>
<span data-ttu-id="08ab7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08ab7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08ab7-108">Permission type</span></span>      | <span data-ttu-id="08ab7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08ab7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ab7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08ab7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08ab7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08ab7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08ab7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08ab7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ab7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ab7-113">Not supported.</span></span>    |
|<span data-ttu-id="08ab7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08ab7-114">Application</span></span> | <span data-ttu-id="08ab7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ab7-115">Not supported.</span></span> |

<span data-ttu-id="08ab7-116">**Примечание:** Пользователи, группы и контакты — это типы объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="08ab7-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="08ab7-117">В результате, если необходимо удалить пользователей, можно использовать следующее разрешение: User. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="08ab7-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="08ab7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08ab7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="08ab7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08ab7-119">Request headers</span></span>
| <span data-ttu-id="08ab7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="08ab7-120">Name</span></span>       | <span data-ttu-id="08ab7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="08ab7-121">Type</span></span> | <span data-ttu-id="08ab7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08ab7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08ab7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ab7-123">Authorization</span></span>  | <span data-ttu-id="08ab7-124">string</span><span class="sxs-lookup"><span data-stu-id="08ab7-124">string</span></span>  | <span data-ttu-id="08ab7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08ab7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08ab7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08ab7-127">Request body</span></span>
<span data-ttu-id="08ab7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08ab7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ab7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="08ab7-129">Response</span></span>

<span data-ttu-id="08ab7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08ab7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08ab7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="08ab7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08ab7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="08ab7-133">Request</span></span>
<span data-ttu-id="08ab7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08ab7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="08ab7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="08ab7-135">Response</span></span>
<span data-ttu-id="08ab7-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08ab7-136">Here is an example of the response.</span></span> 
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
