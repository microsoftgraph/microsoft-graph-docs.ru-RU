---
title: Удаление параметра группы
description: Удаление параметра группы.
ms.openlocfilehash: 1c8a62225497aed066a2a25630103b0ee46b3963
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025831"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="1e901-103">Удаление параметра группы</span><span class="sxs-lookup"><span data-stu-id="1e901-103">Delete a group setting</span></span>

<span data-ttu-id="1e901-104">Удаление параметра группы.</span><span class="sxs-lookup"><span data-stu-id="1e901-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e901-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e901-105">Permissions</span></span>

<span data-ttu-id="1e901-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e901-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e901-108">Permission type</span></span>      | <span data-ttu-id="1e901-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e901-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e901-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e901-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e901-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e901-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e901-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e901-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e901-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e901-113">Not supported.</span></span>    |
|<span data-ttu-id="1e901-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e901-114">Application</span></span> | <span data-ttu-id="1e901-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e901-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e901-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e901-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="1e901-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e901-117">Request headers</span></span>

| <span data-ttu-id="1e901-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1e901-118">Name</span></span> | <span data-ttu-id="1e901-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1e901-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1e901-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e901-120">Authorization</span></span>  | <span data-ttu-id="1e901-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e901-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e901-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e901-123">Content-Type</span></span>  | <span data-ttu-id="1e901-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e901-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e901-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e901-125">Request body</span></span>
<span data-ttu-id="1e901-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e901-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e901-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e901-127">Response</span></span>

<span data-ttu-id="1e901-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1e901-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e901-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1e901-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e901-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e901-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="1e901-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e901-132">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->