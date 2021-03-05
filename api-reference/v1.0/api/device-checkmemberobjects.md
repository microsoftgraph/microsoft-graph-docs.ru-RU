---
title: 'устройство: checkMemberObjects'
description: Проверьте членство в списке групп или ролей каталога для указанного объекта устройства.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3abeb1822efb34af9d46a9d0b4577885f2f82c96
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448865"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="754ec-103">устройство: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="754ec-103">device: checkMemberObjects</span></span>

<span data-ttu-id="754ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="754ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="754ec-105">Проверьте членство в списке групп или ролей каталога для указанного объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="754ec-105">Check for membership in a list of groups or directory roles for the specified device object.</span></span> <span data-ttu-id="754ec-106">Этот метод является транзитным.</span><span class="sxs-lookup"><span data-stu-id="754ec-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="754ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="754ec-107">Permissions</span></span>

<span data-ttu-id="754ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="754ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="754ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="754ec-110">Permission type</span></span>                        | <span data-ttu-id="754ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="754ec-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="754ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="754ec-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="754ec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="754ec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="754ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="754ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="754ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="754ec-115">Not supported.</span></span> |
| <span data-ttu-id="754ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="754ec-116">Application</span></span>                            | <span data-ttu-id="754ec-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="754ec-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="754ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="754ec-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="754ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="754ec-119">Request headers</span></span>

| <span data-ttu-id="754ec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="754ec-120">Name</span></span>          | <span data-ttu-id="754ec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="754ec-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="754ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="754ec-122">Authorization</span></span> | <span data-ttu-id="754ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="754ec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="754ec-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="754ec-125">Content-Type</span></span>  | <span data-ttu-id="754ec-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="754ec-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="754ec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="754ec-128">Request body</span></span>

<span data-ttu-id="754ec-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="754ec-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="754ec-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="754ec-130">Parameter</span></span>    | <span data-ttu-id="754ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="754ec-131">Type</span></span>        | <span data-ttu-id="754ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="754ec-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="754ec-133">ids</span><span class="sxs-lookup"><span data-stu-id="754ec-133">ids</span></span> | <span data-ttu-id="754ec-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="754ec-134">String collection</span></span> | <span data-ttu-id="754ec-135">Коллекция, которая содержит объектные ID групп, роли каталога или roleTemplate ID ролей каталога, в которых необходимо проверить членство.</span><span class="sxs-lookup"><span data-stu-id="754ec-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="754ec-136">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="754ec-136">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="754ec-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="754ec-137">Response</span></span>

<span data-ttu-id="754ec-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="754ec-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="754ec-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="754ec-139">Examples</span></span>

<span data-ttu-id="754ec-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="754ec-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="754ec-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="754ec-141">Request</span></span>

<span data-ttu-id="754ec-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="754ec-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="754ec-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="754ec-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/devices/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="754ec-144">C#</span><span class="sxs-lookup"><span data-stu-id="754ec-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/device-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="754ec-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="754ec-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/device-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="754ec-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="754ec-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/device-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="754ec-147">Java</span><span class="sxs-lookup"><span data-stu-id="754ec-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/device-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="754ec-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="754ec-148">Response</span></span>

<span data-ttu-id="754ec-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="754ec-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="754ec-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="754ec-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

