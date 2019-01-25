---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0efbfe2aa06579a5c52c2cee1020e0269bc0265f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523010"
---
# <a name="delete-device"></a><span data-ttu-id="656f1-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="656f1-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656f1-104">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="656f1-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="656f1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="656f1-105">Permissions</span></span>
<span data-ttu-id="656f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="656f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="656f1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="656f1-108">Permission type</span></span>      | <span data-ttu-id="656f1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="656f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="656f1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="656f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="656f1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="656f1-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="656f1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="656f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="656f1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="656f1-113">Not supported.</span></span>    |
|<span data-ttu-id="656f1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="656f1-114">Application</span></span> | <span data-ttu-id="656f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="656f1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="656f1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="656f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="656f1-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="656f1-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="656f1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="656f1-118">Request headers</span></span>
| <span data-ttu-id="656f1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="656f1-119">Name</span></span>       | <span data-ttu-id="656f1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="656f1-120">Type</span></span> | <span data-ttu-id="656f1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="656f1-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="656f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="656f1-122">Authorization</span></span>  | <span data-ttu-id="656f1-123">string</span><span class="sxs-lookup"><span data-stu-id="656f1-123">string</span></span>  | <span data-ttu-id="656f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="656f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="656f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="656f1-126">Request body</span></span>
<span data-ttu-id="656f1-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="656f1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="656f1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="656f1-128">Response</span></span>

<span data-ttu-id="656f1-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="656f1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="656f1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="656f1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="656f1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="656f1-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="656f1-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="656f1-133">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
