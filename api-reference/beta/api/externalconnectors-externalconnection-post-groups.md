---
title: Создание externalGroup
description: Создайте новый объект externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 128396676462bcf2231f566b7a9830d58ddbc2c8
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467697"
---
# <a name="create-externalgroup"></a><span data-ttu-id="8d20c-103">Создание externalGroup</span><span class="sxs-lookup"><span data-stu-id="8d20c-103">Create externalGroup</span></span>

<span data-ttu-id="8d20c-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="8d20c-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d20c-105">Создайте новый [объект externalGroup.](../resources/externalconnectors-externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8d20c-105">Create a new [externalGroup](../resources/externalconnectors-externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d20c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d20c-106">Permissions</span></span>

<span data-ttu-id="8d20c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d20c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d20c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d20c-109">Permission type</span></span>                        | <span data-ttu-id="8d20c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d20c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d20c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d20c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d20c-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8d20c-112">Not supported</span></span>                               |
| <span data-ttu-id="8d20c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d20c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d20c-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8d20c-114">Not supported</span></span>                               |
| <span data-ttu-id="8d20c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d20c-115">Application</span></span>                            | <span data-ttu-id="8d20c-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d20c-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="8d20c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d20c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="8d20c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d20c-118">Request headers</span></span>

| <span data-ttu-id="8d20c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d20c-119">Name</span></span>          | <span data-ttu-id="8d20c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d20c-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="8d20c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d20c-121">Authorization</span></span> | <span data-ttu-id="8d20c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d20c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8d20c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d20c-124">Content-Type</span></span>  | <span data-ttu-id="8d20c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d20c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d20c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d20c-127">Request body</span></span>

<span data-ttu-id="8d20c-128">В теле запроса поставляем представление JSON объекта [externalGroup.](../resources/externalconnectors-externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8d20c-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalconnectors-externalgroup.md) object.</span></span>

<span data-ttu-id="8d20c-129">В следующей таблице показаны свойства, необходимые при создании [externalGroup.](../resources/externalconnectors-externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8d20c-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalconnectors-externalgroup.md).</span></span>

| <span data-ttu-id="8d20c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d20c-130">Property</span></span>    | <span data-ttu-id="8d20c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d20c-131">Type</span></span>   | <span data-ttu-id="8d20c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d20c-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8d20c-133">id</span><span class="sxs-lookup"><span data-stu-id="8d20c-133">id</span></span>          | <span data-ttu-id="8d20c-134">String</span><span class="sxs-lookup"><span data-stu-id="8d20c-134">String</span></span> | <span data-ttu-id="8d20c-135">Уникальный ID внешней группы в подключении.</span><span class="sxs-lookup"><span data-stu-id="8d20c-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="8d20c-136">Он должен быть альфа-числом и может иметь длину до 128 символов.</span><span class="sxs-lookup"><span data-stu-id="8d20c-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="8d20c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8d20c-137">displayName</span></span> | <span data-ttu-id="8d20c-138">String</span><span class="sxs-lookup"><span data-stu-id="8d20c-138">String</span></span> | <span data-ttu-id="8d20c-139">Дружеское имя внешней группы.</span><span class="sxs-lookup"><span data-stu-id="8d20c-139">The friendly name of the external group.</span></span> <span data-ttu-id="8d20c-140">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8d20c-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="8d20c-141">description</span><span class="sxs-lookup"><span data-stu-id="8d20c-141">description</span></span> | <span data-ttu-id="8d20c-142">String</span><span class="sxs-lookup"><span data-stu-id="8d20c-142">String</span></span> | <span data-ttu-id="8d20c-143">Описание внешней группы.</span><span class="sxs-lookup"><span data-stu-id="8d20c-143">The description of the external group.</span></span> <span data-ttu-id="8d20c-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8d20c-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="8d20c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d20c-145">Response</span></span>

<span data-ttu-id="8d20c-146">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект externalGroup](../resources/externalconnectors-externalgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8d20c-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalconnectors-externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d20c-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d20c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d20c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d20c-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8d20c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d20c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[<span data-ttu-id="8d20c-150">C#</span><span class="sxs-lookup"><span data-stu-id="8d20c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d20c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d20c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d20c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d20c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d20c-153">Java</span><span class="sxs-lookup"><span data-stu-id="8d20c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8d20c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d20c-154">Response</span></span>

<span data-ttu-id="8d20c-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d20c-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
