---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 51adc59b901a2a639360fe12c8a80e2fe6114808
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276386"
---
# <a name="delete-device"></a><span data-ttu-id="2ef98-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="2ef98-103">Delete device</span></span>

<span data-ttu-id="2ef98-104">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="2ef98-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ef98-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef98-105">Permissions</span></span>
<span data-ttu-id="2ef98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ef98-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef98-108">Permission type</span></span>      | <span data-ttu-id="2ef98-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ef98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef98-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef98-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ef98-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2ef98-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef98-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef98-113">Not supported.</span></span>    |
|<span data-ttu-id="2ef98-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef98-114">Application</span></span> | <span data-ttu-id="2ef98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef98-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef98-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef98-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="2ef98-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="2ef98-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ef98-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef98-118">Request headers</span></span>
| <span data-ttu-id="2ef98-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef98-119">Name</span></span>       | <span data-ttu-id="2ef98-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef98-120">Type</span></span> | <span data-ttu-id="2ef98-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef98-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ef98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef98-122">Authorization</span></span>  | <span data-ttu-id="2ef98-123">string</span><span class="sxs-lookup"><span data-stu-id="2ef98-123">string</span></span>  | <span data-ttu-id="2ef98-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ef98-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ef98-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ef98-126">Request body</span></span>
<span data-ttu-id="2ef98-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ef98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ef98-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ef98-128">Response</span></span>

<span data-ttu-id="2ef98-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ef98-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef98-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ef98-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ef98-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef98-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="2ef98-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef98-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ef98-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2ef98-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ef98-135">C#</span><span class="sxs-lookup"><span data-stu-id="2ef98-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ef98-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ef98-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2ef98-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2ef98-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
