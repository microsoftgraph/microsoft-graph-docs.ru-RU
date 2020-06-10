---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a258b33c40d56537ecf833b2b5f91e110af898e1
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681091"
---
# <a name="create-registereduser"></a><span data-ttu-id="c69ab-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="c69ab-103">Create registeredUser</span></span>

<span data-ttu-id="c69ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c69ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c69ab-105">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="c69ab-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="c69ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c69ab-106">Permissions</span></span>
<span data-ttu-id="c69ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c69ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c69ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c69ab-109">Permission type</span></span>      | <span data-ttu-id="c69ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c69ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c69ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c69ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c69ab-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c69ab-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c69ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c69ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c69ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c69ab-114">Not supported.</span></span>    |
|<span data-ttu-id="c69ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c69ab-115">Application</span></span> | <span data-ttu-id="c69ab-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69ab-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c69ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c69ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c69ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c69ab-118">Request headers</span></span>
| <span data-ttu-id="c69ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c69ab-119">Name</span></span>       | <span data-ttu-id="c69ab-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c69ab-120">Type</span></span> | <span data-ttu-id="c69ab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c69ab-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c69ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c69ab-122">Authorization</span></span>  | <span data-ttu-id="c69ab-123">string</span><span class="sxs-lookup"><span data-stu-id="c69ab-123">string</span></span>  | <span data-ttu-id="c69ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c69ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c69ab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c69ab-126">Request body</span></span>
<span data-ttu-id="c69ab-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c69ab-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c69ab-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c69ab-128">Response</span></span>

<span data-ttu-id="c69ab-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c69ab-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c69ab-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c69ab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c69ab-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c69ab-131">Request</span></span>
<span data-ttu-id="c69ab-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c69ab-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c69ab-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c69ab-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="c69ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c69ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c69ab-135">C#</span><span class="sxs-lookup"><span data-stu-id="c69ab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c69ab-136">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c69ab-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c69ab-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c69ab-137">Response</span></span>
<span data-ttu-id="c69ab-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c69ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
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
