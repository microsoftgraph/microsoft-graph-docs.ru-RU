---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: lleonard-msft
ms.openlocfilehash: dec525e72b523e7bbe95996d4c863c68e01baa15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313204"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="50a15-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="50a15-103">Delete directoryObject</span></span>

<span data-ttu-id="50a15-104">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="50a15-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a15-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50a15-105">Permissions</span></span>
<span data-ttu-id="50a15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="50a15-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50a15-108">Permission type</span></span>      | <span data-ttu-id="50a15-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50a15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a15-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50a15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50a15-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50a15-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50a15-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50a15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a15-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a15-113">Not supported.</span></span>    |
|<span data-ttu-id="50a15-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50a15-114">Application</span></span> | <span data-ttu-id="50a15-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50a15-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50a15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="50a15-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50a15-117">Request headers</span></span>
| <span data-ttu-id="50a15-118">Имя</span><span class="sxs-lookup"><span data-stu-id="50a15-118">Name</span></span>       | <span data-ttu-id="50a15-119">Тип</span><span class="sxs-lookup"><span data-stu-id="50a15-119">Type</span></span> | <span data-ttu-id="50a15-120">Описание</span><span class="sxs-lookup"><span data-stu-id="50a15-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50a15-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a15-121">Authorization</span></span>  | <span data-ttu-id="50a15-122">string</span><span class="sxs-lookup"><span data-stu-id="50a15-122">string</span></span>  | <span data-ttu-id="50a15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50a15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50a15-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50a15-125">Request body</span></span>
<span data-ttu-id="50a15-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50a15-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a15-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="50a15-127">Response</span></span>

<span data-ttu-id="50a15-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="50a15-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a15-130">Пример</span><span class="sxs-lookup"><span data-stu-id="50a15-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50a15-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="50a15-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="50a15-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="50a15-132">Response</span></span>

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