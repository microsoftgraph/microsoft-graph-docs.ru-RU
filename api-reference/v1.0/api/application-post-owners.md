---
title: Добавление владельца
description: Добавьте владельца в приложение.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c4cebe3c5b35e44d5d81289dbc77cd78332350e7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958645"
---
# <a name="add-owner"></a><span data-ttu-id="95a28-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="95a28-103">Add owner</span></span>

<span data-ttu-id="95a28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95a28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95a28-105">Добавьте владельца в [приложение,](../resources/application.md) разместив его в коллекции владельцев.</span><span class="sxs-lookup"><span data-stu-id="95a28-105">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="95a28-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95a28-106">Permissions</span></span>
<span data-ttu-id="95a28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95a28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95a28-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95a28-109">Permission type</span></span>      | <span data-ttu-id="95a28-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95a28-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95a28-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95a28-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="95a28-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95a28-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95a28-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95a28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95a28-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95a28-114">Not supported.</span></span>    |
|<span data-ttu-id="95a28-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95a28-115">Application</span></span> | <span data-ttu-id="95a28-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="95a28-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

> <span data-ttu-id="95a28-117">**Примечание.** **Application.ReadWrite.OwnedBy** будет недостаточно для добавления другого владельца.</span><span class="sxs-lookup"><span data-stu-id="95a28-117">**Note:** **Application.ReadWrite.OwnedBy** will not be sufficient to add another owner.</span></span> <span data-ttu-id="95a28-118">Согласие также **на application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="95a28-118">Consent also to **Application.ReadWrite.All**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="95a28-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95a28-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="95a28-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95a28-120">Request headers</span></span>
| <span data-ttu-id="95a28-121">Имя</span><span class="sxs-lookup"><span data-stu-id="95a28-121">Name</span></span> | <span data-ttu-id="95a28-122">Описание</span><span class="sxs-lookup"><span data-stu-id="95a28-122">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="95a28-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95a28-123">Authorization</span></span> | <span data-ttu-id="95a28-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a28-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95a28-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95a28-126">Request body</span></span>
<span data-ttu-id="95a28-127">В теле запроса укажи идентификатор объекта каталога, назначенного в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="95a28-127">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="95a28-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a28-128">Response</span></span>

<span data-ttu-id="95a28-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95a28-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="95a28-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95a28-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="95a28-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95a28-131">Request</span></span>
<span data-ttu-id="95a28-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95a28-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="95a28-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="95a28-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="95a28-134">C#</span><span class="sxs-lookup"><span data-stu-id="95a28-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95a28-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95a28-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95a28-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95a28-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95a28-137">Java</span><span class="sxs-lookup"><span data-stu-id="95a28-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95a28-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a28-138">Response</span></span>

<span data-ttu-id="95a28-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95a28-139">The following is an example of the response.</span></span>

><span data-ttu-id="95a28-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95a28-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

