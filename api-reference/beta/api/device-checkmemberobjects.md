---
title: 'Device: Чеккмемберобжектс'
description: Проверка членства в списке групп, ролей каталогов или административных единиц для указанного объекта Device.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aaed357620258430f2c84d35842612326368ca10
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387064"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="1f9cf-103">Device: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="1f9cf-103">device: checkMemberObjects</span></span>

<span data-ttu-id="1f9cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f9cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f9cf-105">Проверка членства в списке групп или административных единиц для указанного объекта Device.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-105">Check for membership in a list of groups or administrative units for the specified device object.</span></span> <span data-ttu-id="1f9cf-106">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f9cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f9cf-107">Permissions</span></span>

<span data-ttu-id="1f9cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f9cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f9cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f9cf-110">Permission type</span></span>                        | <span data-ttu-id="1f9cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f9cf-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f9cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f9cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f9cf-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f9cf-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1f9cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f9cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f9cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-115">Not supported.</span></span> |
| <span data-ttu-id="1f9cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f9cf-116">Application</span></span>                            | <span data-ttu-id="1f9cf-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f9cf-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f9cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f9cf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="1f9cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f9cf-119">Request headers</span></span>

| <span data-ttu-id="1f9cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1f9cf-120">Name</span></span>          | <span data-ttu-id="1f9cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1f9cf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f9cf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f9cf-122">Authorization</span></span> | <span data-ttu-id="1f9cf-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1f9cf-123">Bearer {token}</span></span> |
| <span data-ttu-id="1f9cf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f9cf-124">Content-Type</span></span>  | <span data-ttu-id="1f9cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f9cf-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f9cf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f9cf-126">Request body</span></span>

<span data-ttu-id="1f9cf-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1f9cf-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="1f9cf-128">Parameter</span></span>    | <span data-ttu-id="1f9cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1f9cf-129">Type</span></span>        | <span data-ttu-id="1f9cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1f9cf-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1f9cf-131">ids</span><span class="sxs-lookup"><span data-stu-id="1f9cf-131">ids</span></span> | <span data-ttu-id="1f9cf-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f9cf-132">String collection</span></span> | <span data-ttu-id="1f9cf-133">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов, административных единиц или идентификаторов Ролетемплате ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="1f9cf-134">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-134">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="1f9cf-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f9cf-135">Response</span></span>

<span data-ttu-id="1f9cf-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f9cf-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f9cf-137">Examples</span></span>

<span data-ttu-id="1f9cf-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1f9cf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f9cf-139">Request</span></span>

<span data-ttu-id="1f9cf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f9cf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f9cf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/devices/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="1f9cf-142">C#</span><span class="sxs-lookup"><span data-stu-id="1f9cf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/device-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f9cf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f9cf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/device-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f9cf-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f9cf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/device-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f9cf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f9cf-145">Response</span></span>

<span data-ttu-id="1f9cf-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-146">The following is an example of the response.</span></span> 

> <span data-ttu-id="1f9cf-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f9cf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
