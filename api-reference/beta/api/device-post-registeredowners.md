---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20c742c6a474917cace63576d715fc972b75057f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996180"
---
# <a name="create-registeredowner"></a><span data-ttu-id="05607-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="05607-103">Create registeredOwner</span></span>

<span data-ttu-id="05607-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05607-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05607-105">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="05607-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="05607-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05607-106">Permissions</span></span>
<span data-ttu-id="05607-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05607-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05607-109">Permission type</span></span>      | <span data-ttu-id="05607-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05607-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05607-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05607-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05607-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05607-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05607-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05607-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05607-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05607-114">Not supported.</span></span>    |
|<span data-ttu-id="05607-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05607-115">Application</span></span> | <span data-ttu-id="05607-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05607-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05607-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05607-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="05607-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05607-118">Request headers</span></span>
| <span data-ttu-id="05607-119">Имя</span><span class="sxs-lookup"><span data-stu-id="05607-119">Name</span></span>       | <span data-ttu-id="05607-120">Тип</span><span class="sxs-lookup"><span data-stu-id="05607-120">Type</span></span> | <span data-ttu-id="05607-121">Описание</span><span class="sxs-lookup"><span data-stu-id="05607-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05607-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05607-122">Authorization</span></span>  | <span data-ttu-id="05607-123">string</span><span class="sxs-lookup"><span data-stu-id="05607-123">string</span></span>  | <span data-ttu-id="05607-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05607-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05607-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05607-126">Request body</span></span>
<span data-ttu-id="05607-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05607-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05607-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="05607-128">Response</span></span>

<span data-ttu-id="05607-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="05607-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05607-130">Пример</span><span class="sxs-lookup"><span data-stu-id="05607-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05607-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="05607-131">Request</span></span>
<span data-ttu-id="05607-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05607-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05607-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="05607-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="05607-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05607-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="05607-135">C#</span><span class="sxs-lookup"><span data-stu-id="05607-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05607-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05607-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="05607-137">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05607-137">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="05607-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="05607-138">Response</span></span>
<span data-ttu-id="05607-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05607-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


