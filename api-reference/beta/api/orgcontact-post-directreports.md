---
title: Создание directReport
description: Используйте этот API для создания нового directReport.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f20b584607518e3dd96ffaed748df8a94e90818
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445312"
---
# <a name="create-directreport"></a><span data-ttu-id="03982-103">Создание directReport</span><span class="sxs-lookup"><span data-stu-id="03982-103">Create directReport</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03982-104">Используйте этот API для создания нового directReport.</span><span class="sxs-lookup"><span data-stu-id="03982-104">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="03982-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03982-105">Permissions</span></span>
<span data-ttu-id="03982-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03982-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03982-108">Permission type</span></span>      | <span data-ttu-id="03982-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03982-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03982-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03982-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03982-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03982-111">Not supported.</span></span>    |
|<span data-ttu-id="03982-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03982-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03982-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03982-113">Not supported.</span></span>    |
|<span data-ttu-id="03982-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03982-114">Application</span></span> | <span data-ttu-id="03982-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03982-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03982-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03982-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="03982-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03982-117">Request headers</span></span>
| <span data-ttu-id="03982-118">Имя</span><span class="sxs-lookup"><span data-stu-id="03982-118">Name</span></span>       | <span data-ttu-id="03982-119">Тип</span><span class="sxs-lookup"><span data-stu-id="03982-119">Type</span></span> | <span data-ttu-id="03982-120">Описание</span><span class="sxs-lookup"><span data-stu-id="03982-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03982-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03982-121">Authorization</span></span>  | <span data-ttu-id="03982-122">string</span><span class="sxs-lookup"><span data-stu-id="03982-122">string</span></span>  | <span data-ttu-id="03982-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03982-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03982-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03982-125">Request body</span></span>
<span data-ttu-id="03982-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03982-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03982-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="03982-127">Response</span></span>

<span data-ttu-id="03982-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03982-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03982-129">Пример</span><span class="sxs-lookup"><span data-stu-id="03982-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03982-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="03982-130">Request</span></span>
<span data-ttu-id="03982-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03982-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03982-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="03982-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03982-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="03982-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="03982-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03982-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03982-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03982-135">Response</span></span>
<span data-ttu-id="03982-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03982-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
