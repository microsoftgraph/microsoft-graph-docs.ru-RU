---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cc11432dbf7b54afde7b46ca70fb1c23726cab44
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046939"
---
# <a name="create-registeredowner"></a><span data-ttu-id="cf7b7-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="cf7b7-103">Create registeredOwner</span></span>

<span data-ttu-id="cf7b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf7b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf7b7-105">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf7b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf7b7-106">Permissions</span></span>
<span data-ttu-id="cf7b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cf7b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf7b7-109">Permission type</span></span>      | <span data-ttu-id="cf7b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf7b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf7b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf7b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf7b7-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf7b7-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf7b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf7b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf7b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-114">Not supported.</span></span>    |
|<span data-ttu-id="cf7b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf7b7-115">Application</span></span> | <span data-ttu-id="cf7b7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf7b7-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf7b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf7b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="cf7b7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf7b7-118">Request headers</span></span>
| <span data-ttu-id="cf7b7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cf7b7-119">Name</span></span>       | <span data-ttu-id="cf7b7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cf7b7-120">Type</span></span> | <span data-ttu-id="cf7b7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cf7b7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf7b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf7b7-122">Authorization</span></span>  | <span data-ttu-id="cf7b7-123">string</span><span class="sxs-lookup"><span data-stu-id="cf7b7-123">string</span></span>  | <span data-ttu-id="cf7b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf7b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf7b7-126">Request body</span></span>
<span data-ttu-id="cf7b7-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf7b7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf7b7-128">Response</span></span>

<span data-ttu-id="cf7b7-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf7b7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cf7b7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf7b7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf7b7-131">Request</span></span>
<span data-ttu-id="cf7b7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf7b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf7b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device_1"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cf7b7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf7b7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf7b7-135">C#</span><span class="sxs-lookup"><span data-stu-id="cf7b7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf7b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf7b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf7b7-137">Java</span><span class="sxs-lookup"><span data-stu-id="cf7b7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cf7b7-138">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cf7b7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf7b7-139">Response</span></span>
<span data-ttu-id="cf7b7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-140">Here is an example of the response.</span></span> <span data-ttu-id="cf7b7-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf7b7-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


