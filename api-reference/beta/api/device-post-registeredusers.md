---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb541ca5c15fc771978d6d8fa838de7862b6c7dc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963409"
---
# <a name="create-registereduser"></a><span data-ttu-id="39c74-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="39c74-103">Create registeredUser</span></span>

<span data-ttu-id="39c74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39c74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39c74-105">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="39c74-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="39c74-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39c74-106">Permissions</span></span>
<span data-ttu-id="39c74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="39c74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39c74-109">Permission type</span></span>      | <span data-ttu-id="39c74-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39c74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39c74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39c74-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39c74-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39c74-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39c74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39c74-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39c74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39c74-114">Not supported.</span></span>    |
|<span data-ttu-id="39c74-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="39c74-115">Application</span></span> | <span data-ttu-id="39c74-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39c74-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39c74-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39c74-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="39c74-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39c74-118">Request headers</span></span>
| <span data-ttu-id="39c74-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39c74-119">Name</span></span>       | <span data-ttu-id="39c74-120">Тип</span><span class="sxs-lookup"><span data-stu-id="39c74-120">Type</span></span> | <span data-ttu-id="39c74-121">Описание</span><span class="sxs-lookup"><span data-stu-id="39c74-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39c74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="39c74-122">Authorization</span></span>  | <span data-ttu-id="39c74-123">string</span><span class="sxs-lookup"><span data-stu-id="39c74-123">string</span></span>  | <span data-ttu-id="39c74-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39c74-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39c74-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39c74-126">Request body</span></span>
<span data-ttu-id="39c74-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39c74-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39c74-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="39c74-128">Response</span></span>

<span data-ttu-id="39c74-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39c74-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39c74-130">Пример</span><span class="sxs-lookup"><span data-stu-id="39c74-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39c74-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="39c74-131">Request</span></span>
<span data-ttu-id="39c74-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39c74-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39c74-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="39c74-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="39c74-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39c74-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="39c74-135">C#</span><span class="sxs-lookup"><span data-stu-id="39c74-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39c74-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39c74-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39c74-137">Java</span><span class="sxs-lookup"><span data-stu-id="39c74-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="39c74-138">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39c74-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="39c74-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="39c74-139">Response</span></span>
<span data-ttu-id="39c74-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39c74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


