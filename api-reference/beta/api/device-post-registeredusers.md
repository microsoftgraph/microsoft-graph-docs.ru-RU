---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 114ff43ffe09ca03c43b509f6963768763f85202
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437088"
---
# <a name="create-registereduser"></a><span data-ttu-id="d0751-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="d0751-103">Create registeredUser</span></span>

<span data-ttu-id="d0751-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0751-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0751-105">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="d0751-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0751-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0751-106">Permissions</span></span>
<span data-ttu-id="d0751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d0751-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0751-109">Permission type</span></span>      | <span data-ttu-id="d0751-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0751-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0751-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0751-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0751-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0751-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0751-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0751-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0751-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0751-114">Not supported.</span></span>    |
|<span data-ttu-id="d0751-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0751-115">Application</span></span> | <span data-ttu-id="d0751-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0751-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0751-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0751-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="d0751-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0751-118">Request headers</span></span>
| <span data-ttu-id="d0751-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d0751-119">Name</span></span>       | <span data-ttu-id="d0751-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d0751-120">Type</span></span> | <span data-ttu-id="d0751-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d0751-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0751-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0751-122">Authorization</span></span>  | <span data-ttu-id="d0751-123">string</span><span class="sxs-lookup"><span data-stu-id="d0751-123">string</span></span>  | <span data-ttu-id="d0751-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0751-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0751-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0751-126">Request body</span></span>
<span data-ttu-id="d0751-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0751-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d0751-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0751-128">Response</span></span>

<span data-ttu-id="d0751-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0751-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0751-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d0751-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0751-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0751-131">Request</span></span>
<span data-ttu-id="d0751-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0751-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0751-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0751-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="d0751-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0751-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d0751-135">C#</span><span class="sxs-lookup"><span data-stu-id="d0751-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0751-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0751-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0751-137">Java</span><span class="sxs-lookup"><span data-stu-id="d0751-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d0751-138">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0751-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d0751-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0751-139">Response</span></span>
<span data-ttu-id="d0751-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


