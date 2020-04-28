---
title: Создание memberOf
description: Используйте этот API для создания нового элемента memberOf.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e7293fcc20400e26f93f9a4e4fd89fa9156ceba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474725"
---
# <a name="create-memberof"></a><span data-ttu-id="fb20e-103">Создание memberOf</span><span class="sxs-lookup"><span data-stu-id="fb20e-103">Create memberOf</span></span>

<span data-ttu-id="fb20e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb20e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb20e-105">Используйте этот API для создания нового элемента memberOf.</span><span class="sxs-lookup"><span data-stu-id="fb20e-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb20e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb20e-106">Permissions</span></span>
<span data-ttu-id="fb20e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb20e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb20e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb20e-109">Permission type</span></span>      | <span data-ttu-id="fb20e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb20e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb20e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb20e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb20e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb20e-112">Not supported.</span></span>    |
|<span data-ttu-id="fb20e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb20e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb20e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb20e-114">Not supported.</span></span>    |
|<span data-ttu-id="fb20e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb20e-115">Application</span></span> | <span data-ttu-id="fb20e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb20e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb20e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb20e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="fb20e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb20e-118">Request headers</span></span>
| <span data-ttu-id="fb20e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fb20e-119">Name</span></span>       | <span data-ttu-id="fb20e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fb20e-120">Type</span></span> | <span data-ttu-id="fb20e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fb20e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb20e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb20e-122">Authorization</span></span>  | <span data-ttu-id="fb20e-123">string</span><span class="sxs-lookup"><span data-stu-id="fb20e-123">string</span></span>  | <span data-ttu-id="fb20e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb20e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb20e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb20e-126">Request body</span></span>
<span data-ttu-id="fb20e-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb20e-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fb20e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb20e-128">Response</span></span>

<span data-ttu-id="fb20e-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb20e-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb20e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb20e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb20e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb20e-131">Request</span></span>
<span data-ttu-id="fb20e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb20e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb20e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb20e-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fb20e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb20e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fb20e-135">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb20e-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fb20e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb20e-136">Response</span></span>
<span data-ttu-id="fb20e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb20e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
