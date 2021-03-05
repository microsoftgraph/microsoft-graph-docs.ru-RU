---
title: Удаление administrativeUnit
description: Удаление администратораUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 89bf0f3f5f66c18fe56c12da6859a4b9ec2a658a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442581"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="c4cf0-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c4cf0-103">Delete administrativeUnit</span></span>

<span data-ttu-id="c4cf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4cf0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4cf0-105">Удаление [администратораUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="c4cf0-105">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4cf0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cf0-106">Permissions</span></span>
<span data-ttu-id="c4cf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4cf0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cf0-109">Permission type</span></span>      | <span data-ttu-id="c4cf0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4cf0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4cf0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4cf0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4cf0-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4cf0-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4cf0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4cf0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4cf0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-114">Not supported.</span></span>    |
|<span data-ttu-id="c4cf0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4cf0-115">Application</span></span> | <span data-ttu-id="c4cf0-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4cf0-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4cf0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4cf0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c4cf0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4cf0-118">Request headers</span></span>
| <span data-ttu-id="c4cf0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4cf0-119">Name</span></span>       | <span data-ttu-id="c4cf0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4cf0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4cf0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4cf0-121">Authorization</span></span>  | <span data-ttu-id="c4cf0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4cf0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4cf0-124">Request body</span></span>
<span data-ttu-id="c4cf0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4cf0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4cf0-126">Response</span></span>

<span data-ttu-id="c4cf0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4cf0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c4cf0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4cf0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4cf0-130">Request</span></span>
<span data-ttu-id="c4cf0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4cf0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4cf0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="c4cf0-133">C#</span><span class="sxs-lookup"><span data-stu-id="c4cf0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4cf0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4cf0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4cf0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4cf0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4cf0-136">Java</span><span class="sxs-lookup"><span data-stu-id="c4cf0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="c4cf0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4cf0-137">Response</span></span>
<span data-ttu-id="c4cf0-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4cf0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
