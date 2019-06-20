---
title: 'Чатмессажехостедимаже: GetBytes'
description: Получение двоичного представления размещенного изображения в канале или сообщении чата.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a661dfe7e51680804faaac7df6e32ee5e680d22b
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085840"
---
# <a name="chatmessagehostedimage-getbytes"></a><span data-ttu-id="d85ae-103">Чатмессажехостедимаже: GetBytes</span><span class="sxs-lookup"><span data-stu-id="d85ae-103">chatMessageHostedImage: getBytes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d85ae-104">Получение двоичного представления размещенного [изображения](../resources/chatmessagehostedimage.md) в [сообщении](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="d85ae-104">Get the binary representation of a [hosted image](../resources/chatmessagehostedimage.md) in a [message](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d85ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d85ae-105">Permissions</span></span>

<span data-ttu-id="d85ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d85ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d85ae-108">Permission Type</span></span>|<span data-ttu-id="d85ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d85ae-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d85ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d85ae-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d85ae-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85ae-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="d85ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d85ae-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d85ae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d85ae-113">Not supported.</span></span>|
|<span data-ttu-id="d85ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d85ae-114">Application</span></span>| <span data-ttu-id="d85ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d85ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d85ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d85ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}/$value
GET /chats/{id}/messages/{id}/hostedImages/{id}/$value
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d85ae-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d85ae-117">Optional query parameters</span></span>

<span data-ttu-id="d85ae-118">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d85ae-118">This method does not support the [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d85ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d85ae-119">Request headers</span></span>

| <span data-ttu-id="d85ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d85ae-120">Header</span></span>       | <span data-ttu-id="d85ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d85ae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d85ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d85ae-122">Authorization</span></span>  | <span data-ttu-id="d85ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d85ae-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d85ae-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d85ae-125">Request body</span></span>

<span data-ttu-id="d85ae-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d85ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d85ae-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d85ae-127">Response</span></span>

<span data-ttu-id="d85ae-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные запрошенного изображения.</span><span class="sxs-lookup"><span data-stu-id="d85ae-128">If successful, this method returns a `200 OK` response code and binary data of the requested image.</span></span>

## <a name="example"></a><span data-ttu-id="d85ae-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d85ae-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d85ae-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d85ae-130">Request</span></span>

<span data-ttu-id="d85ae-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d85ae-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->

```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
```

##### <a name="response"></a><span data-ttu-id="d85ae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d85ae-132">Response</span></span>

<span data-ttu-id="d85ae-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d85ae-133">Here is an example of the response.</span></span>

><span data-ttu-id="d85ae-134">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d85ae-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="d85ae-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d85ae-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bytes of a hosted image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-getbytes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
