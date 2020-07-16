---
title: Удаление registeredowners
description: Удаление пользователя в качестве зарегистрированного владельца устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f958a1af94d74b9eee3db8f925ed1d6d9246617
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146867"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="913d3-103">Удаление registeredOwner</span><span class="sxs-lookup"><span data-stu-id="913d3-103">Delete registeredOwner</span></span>

<span data-ttu-id="913d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="913d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="913d3-105">Удаление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="913d3-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="913d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="913d3-106">Permissions</span></span>

<span data-ttu-id="913d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="913d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="913d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="913d3-109">Permission type</span></span>      | <span data-ttu-id="913d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="913d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="913d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="913d3-111">Delegated (work or school account)</span></span> |<span data-ttu-id="913d3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="913d3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="913d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="913d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="913d3-114">Not supported.</span></span>    |
|<span data-ttu-id="913d3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="913d3-115">Application</span></span> | <span data-ttu-id="913d3-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="913d3-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="913d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="913d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="913d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="913d3-118">Request headers</span></span>
| <span data-ttu-id="913d3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="913d3-119">Name</span></span>       | <span data-ttu-id="913d3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="913d3-120">Type</span></span> | <span data-ttu-id="913d3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="913d3-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="913d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="913d3-122">Authorization</span></span>  | <span data-ttu-id="913d3-123">string</span><span class="sxs-lookup"><span data-stu-id="913d3-123">string</span></span>  | <span data-ttu-id="913d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="913d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="913d3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="913d3-126">Request body</span></span>
<span data-ttu-id="913d3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="913d3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="913d3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="913d3-128">Response</span></span>

<span data-ttu-id="913d3-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="913d3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="913d3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="913d3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="913d3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="913d3-131">Request</span></span>
<span data-ttu-id="913d3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="913d3-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="913d3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="913d3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```

---

##### <a name="response"></a><span data-ttu-id="913d3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="913d3-134">Response</span></span>
<span data-ttu-id="913d3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="913d3-135">Here is an example of the response.</span></span>
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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
