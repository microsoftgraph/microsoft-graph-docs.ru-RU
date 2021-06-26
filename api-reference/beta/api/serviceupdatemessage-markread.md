---
title: 'serviceUpdateMessage: markRead'
description: Пометить список сообщений об обновлении службы в качестве чтения для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 6df66f75143a719cfa1e6ff3cd507a2a73122438
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151729"
---
# <a name="serviceupdatemessage-markread"></a><span data-ttu-id="fa94b-103">serviceUpdateMessage: markRead</span><span class="sxs-lookup"><span data-stu-id="fa94b-103">serviceUpdateMessage: markRead</span></span>
<span data-ttu-id="fa94b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa94b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa94b-105">Пометить список [serviceUpdateMessages](../resources/serviceupdatemessage.md) в качестве чтения для подписанного пользователя. </span><span class="sxs-lookup"><span data-stu-id="fa94b-105">Mark a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) as **read** for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa94b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa94b-106">Permissions</span></span>
<span data-ttu-id="fa94b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa94b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa94b-109">Permission type</span></span>|<span data-ttu-id="fa94b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa94b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa94b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa94b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa94b-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="fa94b-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="fa94b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa94b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa94b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa94b-114">Not supported.</span></span>|
|<span data-ttu-id="fa94b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa94b-115">Application</span></span>|<span data-ttu-id="fa94b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fa94b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa94b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa94b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/markRead
```

## <a name="request-headers"></a><span data-ttu-id="fa94b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa94b-118">Request headers</span></span>
|<span data-ttu-id="fa94b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fa94b-119">Name</span></span>|<span data-ttu-id="fa94b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa94b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa94b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa94b-121">Authorization</span></span>|<span data-ttu-id="fa94b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa94b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa94b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa94b-124">Content-Type</span></span>|<span data-ttu-id="fa94b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa94b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa94b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa94b-127">Request body</span></span>
<span data-ttu-id="fa94b-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="fa94b-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="fa94b-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fa94b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fa94b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="fa94b-130">Parameter</span></span>|<span data-ttu-id="fa94b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa94b-131">Type</span></span>|<span data-ttu-id="fa94b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa94b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa94b-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="fa94b-133">messageIds</span></span>|<span data-ttu-id="fa94b-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa94b-134">String collection</span></span>|<span data-ttu-id="fa94b-135">Список ID-сообщений, которые необходимо отметить как чтение.</span><span class="sxs-lookup"><span data-stu-id="fa94b-135">List of message IDs to mark as read.</span></span>|


## <a name="response"></a><span data-ttu-id="fa94b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa94b-136">Response</span></span>

<span data-ttu-id="fa94b-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fa94b-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="fa94b-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="fa94b-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa94b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="fa94b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa94b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa94b-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_markread"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/markRead
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```


### <a name="response"></a><span data-ttu-id="fa94b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa94b-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```