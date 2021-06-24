---
title: 'serviceUpdateMessage: неархивный'
description: Unarchive a list of service update messages for the signed in user.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 79c5b5045200a366e9ce4df24eb21f554ae92c1a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107835"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="5fb3c-103">serviceUpdateMessage: неархивный</span><span class="sxs-lookup"><span data-stu-id="5fb3c-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="5fb3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb3c-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fb3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb3c-106">Permissions</span></span>
<span data-ttu-id="5fb3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fb3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fb3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb3c-109">Permission type</span></span>|<span data-ttu-id="5fb3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fb3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fb3c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fb3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb3c-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="5fb3c-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="5fb3c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fb3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fb3c-114">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="5fb3c-114">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="5fb3c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fb3c-115">Application</span></span>|<span data-ttu-id="5fb3c-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5fb3c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fb3c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fb3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="5fb3c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fb3c-118">Request headers</span></span>
|<span data-ttu-id="5fb3c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5fb3c-119">Name</span></span>|<span data-ttu-id="5fb3c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb3c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5fb3c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fb3c-121">Authorization</span></span>|<span data-ttu-id="5fb3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5fb3c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5fb3c-124">Content-Type</span></span>|<span data-ttu-id="5fb3c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fb3c-127">Request body</span></span>
<span data-ttu-id="5fb3c-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="5fb3c-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5fb3c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5fb3c-130">Parameter</span></span>|<span data-ttu-id="5fb3c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5fb3c-131">Type</span></span>|<span data-ttu-id="5fb3c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb3c-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="5fb3c-133">messageIds</span></span>|<span data-ttu-id="5fb3c-134">Набор строк</span><span class="sxs-lookup"><span data-stu-id="5fb3c-134">String collection</span></span>|<span data-ttu-id="5fb3c-135">Список ID-сообщений для неархивных.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="5fb3c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fb3c-136">Response</span></span>

<span data-ttu-id="5fb3c-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="5fb3c-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="5fb3c-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb3c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="5fb3c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fb3c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fb3c-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_unarchive"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/unarchive
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```


### <a name="response"></a><span data-ttu-id="5fb3c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fb3c-141">Response</span></span>
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