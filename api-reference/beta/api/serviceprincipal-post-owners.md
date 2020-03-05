---
title: 'servicePrincipal: Добавление владельца'
description: Используйте этот API, чтобы добавить владельца для субъекта-службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7379c07d7ba3704fc2e44f2a46744418be54b4af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453351"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="90c11-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="90c11-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="90c11-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90c11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90c11-105">Используйте этот API, чтобы добавить владельца для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="90c11-105">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="90c11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90c11-106">Permissions</span></span>
<span data-ttu-id="90c11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c11-109">Permission type</span></span>      | <span data-ttu-id="90c11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90c11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90c11-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90c11-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90c11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c11-114">Not supported.</span></span>    |
|<span data-ttu-id="90c11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90c11-115">Application</span></span> | <span data-ttu-id="90c11-116">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="90c11-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90c11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="90c11-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90c11-118">Request headers</span></span>
| <span data-ttu-id="90c11-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90c11-119">Name</span></span>       | <span data-ttu-id="90c11-120">Тип</span><span class="sxs-lookup"><span data-stu-id="90c11-120">Type</span></span> | <span data-ttu-id="90c11-121">Описание</span><span class="sxs-lookup"><span data-stu-id="90c11-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90c11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90c11-122">Authorization</span></span>  | <span data-ttu-id="90c11-123">string</span><span class="sxs-lookup"><span data-stu-id="90c11-123">string</span></span>  | <span data-ttu-id="90c11-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90c11-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c11-126">Request body</span></span>
<span data-ttu-id="90c11-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90c11-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90c11-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c11-128">Response</span></span>

<span data-ttu-id="90c11-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90c11-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c11-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90c11-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90c11-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c11-131">Request</span></span>
<span data-ttu-id="90c11-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c11-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90c11-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90c11-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="90c11-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90c11-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="90c11-135">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90c11-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="90c11-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c11-136">Response</span></span>
<span data-ttu-id="90c11-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90c11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
