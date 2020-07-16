---
title: Удаление registeredUsers
description: Удаление пользователя в качестве зарегистрированного пользователя устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40f510c0dd82efb47e0685c0432e2d3b42b2ce9d
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146728"
---
# <a name="delete-registereduser"></a><span data-ttu-id="a885c-103">Удаление экземпляра registereduser</span><span class="sxs-lookup"><span data-stu-id="a885c-103">Delete registeredUser</span></span>

<span data-ttu-id="a885c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a885c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a885c-105">Удаление пользователя в качестве зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="a885c-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="a885c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a885c-106">Permissions</span></span>

<span data-ttu-id="a885c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a885c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a885c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a885c-109">Permission type</span></span>      | <span data-ttu-id="a885c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a885c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a885c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a885c-111">Delegated (work or school account)</span></span> |<span data-ttu-id="a885c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a885c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a885c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a885c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a885c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a885c-114">Not supported.</span></span>    |
|<span data-ttu-id="a885c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a885c-115">Application</span></span> | <span data-ttu-id="a885c-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a885c-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a885c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a885c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a885c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a885c-118">Request headers</span></span>
| <span data-ttu-id="a885c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a885c-119">Name</span></span>       | <span data-ttu-id="a885c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a885c-120">Type</span></span> | <span data-ttu-id="a885c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a885c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a885c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a885c-122">Authorization</span></span>  | <span data-ttu-id="a885c-123">string</span><span class="sxs-lookup"><span data-stu-id="a885c-123">string</span></span>  | <span data-ttu-id="a885c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a885c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a885c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a885c-126">Request body</span></span>
<span data-ttu-id="a885c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a885c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a885c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a885c-128">Response</span></span>

<span data-ttu-id="a885c-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a885c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a885c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a885c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a885c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a885c-131">Request</span></span>
<span data-ttu-id="a885c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a885c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a885c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a885c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/{id}/$ref
```

---

##### <a name="response"></a><span data-ttu-id="a885c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a885c-134">Response</span></span>
<span data-ttu-id="a885c-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a885c-135">Here is an example of the response.</span></span>
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
  "description": "Delete registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
