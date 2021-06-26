---
title: 'serviceUpdateMessage: markUnread'
description: Пометить список сообщений об обновлении службы как непрочитанные для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 9fe68bf8c89aa47d232c4c261a19655e66737419
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151722"
---
# <a name="serviceupdatemessage-markunread"></a><span data-ttu-id="757b1-103">serviceUpdateMessage: markUnread</span><span class="sxs-lookup"><span data-stu-id="757b1-103">serviceUpdateMessage: markUnread</span></span>
<span data-ttu-id="757b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="757b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="757b1-105">Пометить список [serviceUpdateMessages](../resources/serviceupdatemessage.md) как непрочитанные **для** подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="757b1-105">Mark a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) as **unread** for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="757b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="757b1-106">Permissions</span></span>
<span data-ttu-id="757b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="757b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="757b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="757b1-109">Permission type</span></span>|<span data-ttu-id="757b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="757b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="757b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="757b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="757b1-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="757b1-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="757b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="757b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="757b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="757b1-114">Not supported.</span></span>|
|<span data-ttu-id="757b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="757b1-115">Application</span></span>|<span data-ttu-id="757b1-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="757b1-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="757b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="757b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/markUnread
```

## <a name="request-headers"></a><span data-ttu-id="757b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="757b1-118">Request headers</span></span>
|<span data-ttu-id="757b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="757b1-119">Name</span></span>|<span data-ttu-id="757b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="757b1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="757b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="757b1-121">Authorization</span></span>|<span data-ttu-id="757b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="757b1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="757b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="757b1-124">Content-Type</span></span>|<span data-ttu-id="757b1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="757b1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="757b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="757b1-127">Request body</span></span>
<span data-ttu-id="757b1-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="757b1-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="757b1-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="757b1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="757b1-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="757b1-130">Parameter</span></span>|<span data-ttu-id="757b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="757b1-131">Type</span></span>|<span data-ttu-id="757b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="757b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="757b1-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="757b1-133">messageIds</span></span>|<span data-ttu-id="757b1-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="757b1-134">String collection</span></span>|<span data-ttu-id="757b1-135">Список ID-сообщений, которые необходимо отметить как непрочитанные.</span><span class="sxs-lookup"><span data-stu-id="757b1-135">List of message IDs to mark as unread.</span></span>|

## <a name="response"></a><span data-ttu-id="757b1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="757b1-136">Response</span></span>

<span data-ttu-id="757b1-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="757b1-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="757b1-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="757b1-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="757b1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="757b1-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="757b1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="757b1-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_markunread"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/markUnread
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a><span data-ttu-id="757b1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="757b1-141">Response</span></span>
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