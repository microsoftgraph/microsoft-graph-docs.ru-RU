---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7b1a3e13e725df9b344b4612f79aa10fd22429d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336349"
---
# <a name="get-resource"></a><span data-ttu-id="a17ef-103">Вывод ресурса</span><span class="sxs-lookup"><span data-stu-id="a17ef-103">Get resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a17ef-104">Получение двоичных данных объекта [ресурса](../resources/onenoteresource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="a17ef-104">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a17ef-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a17ef-105">Permissions</span></span>
<span data-ttu-id="a17ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a17ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a17ef-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a17ef-108">Permission type</span></span>      | <span data-ttu-id="a17ef-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a17ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a17ef-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a17ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a17ef-111">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a17ef-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a17ef-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a17ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a17ef-113">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a17ef-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a17ef-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a17ef-114">Application</span></span> | <span data-ttu-id="a17ef-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a17ef-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a17ef-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a17ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="a17ef-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a17ef-117">Request headers</span></span>
| <span data-ttu-id="a17ef-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a17ef-118">Name</span></span>       | <span data-ttu-id="a17ef-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a17ef-119">Type</span></span> | <span data-ttu-id="a17ef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a17ef-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a17ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a17ef-121">Authorization</span></span>  | <span data-ttu-id="a17ef-122">string</span><span class="sxs-lookup"><span data-stu-id="a17ef-122">string</span></span>  | <span data-ttu-id="a17ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a17ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a17ef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a17ef-125">Request body</span></span>
<span data-ttu-id="a17ef-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a17ef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a17ef-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a17ef-127">Response</span></span>

<span data-ttu-id="a17ef-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a17ef-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="a17ef-129">Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.</span><span class="sxs-lookup"><span data-stu-id="a17ef-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="a17ef-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a17ef-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a17ef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a17ef-131">Request</span></span>
<span data-ttu-id="a17ef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a17ef-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="a17ef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a17ef-133">Response</span></span>
<span data-ttu-id="a17ef-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a17ef-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
