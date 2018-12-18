---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: tfitzmac
ms.openlocfilehash: ae2f4b458ebd18c366c2b8aecf6b203ff5d42cda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342905"
---
# <a name="delete-device"></a><span data-ttu-id="a1364-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="a1364-103">Delete device</span></span>

<span data-ttu-id="a1364-104">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="a1364-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1364-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1364-105">Permissions</span></span>
<span data-ttu-id="a1364-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a1364-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1364-108">Permission type</span></span>      | <span data-ttu-id="a1364-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1364-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1364-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1364-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1364-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1364-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a1364-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1364-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1364-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1364-113">Not supported.</span></span>    |
|<span data-ttu-id="a1364-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1364-114">Application</span></span> | <span data-ttu-id="a1364-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1364-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1364-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1364-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="a1364-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="a1364-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1364-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1364-118">Request headers</span></span>
| <span data-ttu-id="a1364-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a1364-119">Name</span></span>       | <span data-ttu-id="a1364-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a1364-120">Type</span></span> | <span data-ttu-id="a1364-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a1364-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1364-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1364-122">Authorization</span></span>  | <span data-ttu-id="a1364-123">string</span><span class="sxs-lookup"><span data-stu-id="a1364-123">string</span></span>  | <span data-ttu-id="a1364-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1364-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1364-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1364-126">Request body</span></span>
<span data-ttu-id="a1364-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1364-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1364-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1364-128">Response</span></span>

<span data-ttu-id="a1364-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a1364-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1364-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a1364-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1364-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1364-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="a1364-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1364-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
