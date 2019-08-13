---
title: Создание memberOf
description: Используйте этот API для создания нового элемента memberOf.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac5e3ca84ac35f002133c19a4cbb53c8041717fc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342406"
---
# <a name="create-memberof"></a><span data-ttu-id="0fe1f-103">Создание memberOf</span><span class="sxs-lookup"><span data-stu-id="0fe1f-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fe1f-104">Используйте этот API для создания нового элемента memberOf.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fe1f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fe1f-105">Permissions</span></span>
<span data-ttu-id="0fe1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe1f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fe1f-108">Permission type</span></span>      | <span data-ttu-id="0fe1f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fe1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fe1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0fe1f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-111">Not supported.</span></span>    |
|<span data-ttu-id="0fe1f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fe1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe1f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-113">Not supported.</span></span>    |
|<span data-ttu-id="0fe1f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fe1f-114">Application</span></span> | <span data-ttu-id="0fe1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe1f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fe1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="0fe1f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fe1f-117">Request headers</span></span>
| <span data-ttu-id="0fe1f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0fe1f-118">Name</span></span>       | <span data-ttu-id="0fe1f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0fe1f-119">Type</span></span> | <span data-ttu-id="0fe1f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0fe1f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fe1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fe1f-121">Authorization</span></span>  | <span data-ttu-id="0fe1f-122">string</span><span class="sxs-lookup"><span data-stu-id="0fe1f-122">string</span></span>  | <span data-ttu-id="0fe1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe1f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fe1f-125">Request body</span></span>
<span data-ttu-id="0fe1f-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0fe1f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fe1f-127">Response</span></span>

<span data-ttu-id="0fe1f-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe1f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0fe1f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fe1f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fe1f-130">Request</span></span>
<span data-ttu-id="0fe1f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fe1f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe1f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fe1f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe1f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0fe1f-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0fe1f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fe1f-135">Response</span></span>
<span data-ttu-id="0fe1f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fe1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
