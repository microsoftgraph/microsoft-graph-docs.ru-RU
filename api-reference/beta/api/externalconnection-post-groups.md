---
title: Создание externalGroup
description: Создание объекта externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6ca8968daf3abb98bba66a4146fc3b41c9d54441
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873047"
---
# <a name="create-externalgroup"></a><span data-ttu-id="86814-103">Создание externalGroup</span><span class="sxs-lookup"><span data-stu-id="86814-103">Create externalGroup</span></span>

<span data-ttu-id="86814-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86814-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86814-105">Создание объекта [externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="86814-105">Create a new [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86814-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86814-106">Permissions</span></span>

<span data-ttu-id="86814-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86814-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86814-109">Permission type</span></span>                        | <span data-ttu-id="86814-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86814-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86814-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86814-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86814-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="86814-112">Not supported</span></span>                               |
| <span data-ttu-id="86814-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86814-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86814-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="86814-114">Not supported</span></span>                               |
| <span data-ttu-id="86814-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="86814-115">Application</span></span>                            | <span data-ttu-id="86814-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86814-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="86814-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86814-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="86814-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86814-118">Request headers</span></span>

| <span data-ttu-id="86814-119">Имя</span><span class="sxs-lookup"><span data-stu-id="86814-119">Name</span></span>          | <span data-ttu-id="86814-120">Описание</span><span class="sxs-lookup"><span data-stu-id="86814-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="86814-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86814-121">Authorization</span></span> | <span data-ttu-id="86814-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86814-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="86814-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86814-124">Content-Type</span></span>  | <span data-ttu-id="86814-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86814-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86814-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="86814-127">Request body</span></span>

<span data-ttu-id="86814-128">В теле запроса укажу представление объекта [externalGroup](../resources/externalgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="86814-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalgroup.md) object.</span></span>

<span data-ttu-id="86814-129">В следующей таблице показаны свойства, необходимые при создании [объекта externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="86814-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalgroup.md).</span></span>

| <span data-ttu-id="86814-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86814-130">Property</span></span>    | <span data-ttu-id="86814-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86814-131">Type</span></span>   | <span data-ttu-id="86814-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86814-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="86814-133">id</span><span class="sxs-lookup"><span data-stu-id="86814-133">id</span></span>          | <span data-ttu-id="86814-134">String</span><span class="sxs-lookup"><span data-stu-id="86814-134">String</span></span> | <span data-ttu-id="86814-135">Уникальный ИД внешней группы в соединении.</span><span class="sxs-lookup"><span data-stu-id="86814-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="86814-136">Она должна быть букво-цифрой и длиной до 128 символов.</span><span class="sxs-lookup"><span data-stu-id="86814-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="86814-137">displayName</span><span class="sxs-lookup"><span data-stu-id="86814-137">displayName</span></span> | <span data-ttu-id="86814-138">String</span><span class="sxs-lookup"><span data-stu-id="86814-138">String</span></span> | <span data-ttu-id="86814-139">Имя внешней группы.</span><span class="sxs-lookup"><span data-stu-id="86814-139">The friendly name of the external group.</span></span> <span data-ttu-id="86814-140">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="86814-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="86814-141">description</span><span class="sxs-lookup"><span data-stu-id="86814-141">description</span></span> | <span data-ttu-id="86814-142">String</span><span class="sxs-lookup"><span data-stu-id="86814-142">String</span></span> | <span data-ttu-id="86814-143">Описание внешней группы.</span><span class="sxs-lookup"><span data-stu-id="86814-143">The description of the external group.</span></span> <span data-ttu-id="86814-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="86814-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="86814-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="86814-145">Response</span></span>

<span data-ttu-id="86814-146">В случае успеха этот метод возвращает код отклика и `201 Created` [объект externalGroup](../resources/externalgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86814-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86814-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="86814-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86814-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="86814-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="86814-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="86814-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[<span data-ttu-id="86814-150">C#</span><span class="sxs-lookup"><span data-stu-id="86814-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86814-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86814-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86814-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86814-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86814-153">Java</span><span class="sxs-lookup"><span data-stu-id="86814-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="86814-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="86814-154">Response</span></span>

<span data-ttu-id="86814-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="86814-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
