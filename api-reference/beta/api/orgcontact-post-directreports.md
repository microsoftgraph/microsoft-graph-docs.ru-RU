---
title: Создание directReport
description: Используйте этот API для создания нового directReport.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 380f36b0b100d6f78c74ab0b0244ebe51fac6cde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456243"
---
# <a name="create-directreport"></a><span data-ttu-id="dec04-103">Создание directReport</span><span class="sxs-lookup"><span data-stu-id="dec04-103">Create directReport</span></span>

<span data-ttu-id="dec04-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dec04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dec04-105">Используйте этот API для создания нового directReport.</span><span class="sxs-lookup"><span data-stu-id="dec04-105">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="dec04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dec04-106">Permissions</span></span>
<span data-ttu-id="dec04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dec04-109">Permission type</span></span>      | <span data-ttu-id="dec04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dec04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dec04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dec04-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dec04-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dec04-112">Not supported.</span></span>    |
|<span data-ttu-id="dec04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dec04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dec04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dec04-114">Not supported.</span></span>    |
|<span data-ttu-id="dec04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dec04-115">Application</span></span> | <span data-ttu-id="dec04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dec04-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dec04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dec04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="dec04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dec04-118">Request headers</span></span>
| <span data-ttu-id="dec04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dec04-119">Name</span></span>       | <span data-ttu-id="dec04-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dec04-120">Type</span></span> | <span data-ttu-id="dec04-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dec04-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dec04-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dec04-122">Authorization</span></span>  | <span data-ttu-id="dec04-123">string</span><span class="sxs-lookup"><span data-stu-id="dec04-123">string</span></span>  | <span data-ttu-id="dec04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dec04-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dec04-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dec04-126">Request body</span></span>
<span data-ttu-id="dec04-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dec04-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dec04-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dec04-128">Response</span></span>

<span data-ttu-id="dec04-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dec04-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dec04-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dec04-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dec04-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dec04-131">Request</span></span>
<span data-ttu-id="dec04-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dec04-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dec04-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dec04-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="dec04-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dec04-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dec04-135">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dec04-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dec04-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dec04-136">Response</span></span>
<span data-ttu-id="dec04-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dec04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
