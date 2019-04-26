---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fccafa016dad9892c701e852bc592564661c9cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555103"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="649f7-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="649f7-103">Delete directoryObject</span></span>

<span data-ttu-id="649f7-104">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="649f7-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="649f7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="649f7-105">Permissions</span></span>
<span data-ttu-id="649f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="649f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="649f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="649f7-108">Permission type</span></span>      | <span data-ttu-id="649f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="649f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="649f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="649f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="649f7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="649f7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="649f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="649f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="649f7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="649f7-113">Not supported.</span></span>    |
|<span data-ttu-id="649f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="649f7-114">Application</span></span> | <span data-ttu-id="649f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="649f7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="649f7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="649f7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="649f7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="649f7-117">Request headers</span></span>
| <span data-ttu-id="649f7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="649f7-118">Name</span></span>       | <span data-ttu-id="649f7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="649f7-119">Type</span></span> | <span data-ttu-id="649f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="649f7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="649f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="649f7-121">Authorization</span></span>  | <span data-ttu-id="649f7-122">string</span><span class="sxs-lookup"><span data-stu-id="649f7-122">string</span></span>  | <span data-ttu-id="649f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="649f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="649f7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="649f7-125">Request body</span></span>
<span data-ttu-id="649f7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="649f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="649f7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="649f7-127">Response</span></span>

<span data-ttu-id="649f7-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="649f7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="649f7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="649f7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="649f7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="649f7-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="649f7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="649f7-132">Response</span></span>

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
