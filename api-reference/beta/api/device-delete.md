---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
ms.openlocfilehash: 5635e183a2aebc11e95c5836076ad513075f50d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075688"
---
# <a name="delete-device"></a><span data-ttu-id="3a9e4-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="3a9e4-103">Delete device</span></span>

> <span data-ttu-id="3a9e4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a9e4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a9e4-106">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a9e4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9e4-107">Permissions</span></span>
<span data-ttu-id="3a9e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a9e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9e4-110">Permission type</span></span>      | <span data-ttu-id="3a9e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a9e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a9e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a9e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a9e4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a9e4-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3a9e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a9e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a9e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-115">Not supported.</span></span>    |
|<span data-ttu-id="3a9e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a9e4-116">Application</span></span> | <span data-ttu-id="3a9e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a9e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a9e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="3a9e4-119">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a9e4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a9e4-120">Request headers</span></span>
| <span data-ttu-id="3a9e4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3a9e4-121">Name</span></span>       | <span data-ttu-id="3a9e4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3a9e4-122">Type</span></span> | <span data-ttu-id="3a9e4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3a9e4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a9e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a9e4-124">Authorization</span></span>  | <span data-ttu-id="3a9e4-125">string</span><span class="sxs-lookup"><span data-stu-id="3a9e4-125">string</span></span>  | <span data-ttu-id="3a9e4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a9e4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a9e4-128">Request body</span></span>
<span data-ttu-id="3a9e4-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a9e4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9e4-130">Response</span></span>

<span data-ttu-id="3a9e4-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3a9e4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9e4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3a9e4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a9e4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a9e4-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="3a9e4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a9e4-135">Response</span></span>

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