---
title: Получение ресурса
description: Получение двоичных данных объекта resource файла или изображения.
ms.openlocfilehash: 81c07dca78381ede096c62eba73b0842ae294d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075407"
---
# <a name="get-resource"></a><span data-ttu-id="1be17-103">Получение ресурса</span><span class="sxs-lookup"><span data-stu-id="1be17-103">Get resource</span></span>

> <span data-ttu-id="1be17-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1be17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1be17-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1be17-106">Получение двоичных данных объекта [resource](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="1be17-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1be17-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1be17-107">Permissions</span></span>
<span data-ttu-id="1be17-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1be17-110">Permission type</span></span>      | <span data-ttu-id="1be17-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1be17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1be17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1be17-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1be17-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be17-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1be17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1be17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be17-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1be17-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1be17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1be17-116">Application</span></span> | <span data-ttu-id="1be17-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be17-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1be17-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="1be17-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1be17-119">Request headers</span></span>
| <span data-ttu-id="1be17-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1be17-120">Name</span></span>       | <span data-ttu-id="1be17-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1be17-121">Type</span></span> | <span data-ttu-id="1be17-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1be17-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1be17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be17-123">Authorization</span></span>  | <span data-ttu-id="1be17-124">string</span><span class="sxs-lookup"><span data-stu-id="1be17-124">string</span></span>  | <span data-ttu-id="1be17-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1be17-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1be17-127">Request body</span></span>
<span data-ttu-id="1be17-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1be17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1be17-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1be17-129">Response</span></span>

<span data-ttu-id="1be17-130">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1be17-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="1be17-131">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="1be17-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="1be17-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1be17-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1be17-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be17-133">Request</span></span>
<span data-ttu-id="1be17-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1be17-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="1be17-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be17-135">Response</span></span>
<span data-ttu-id="1be17-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1be17-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
