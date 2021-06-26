---
title: 'serviceUpdateMessage: архив'
description: Архивировать список сообщений об обновлении службы для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: be8dfba8bd5bcbd9d0ccb20a31354a890810ba79
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151750"
---
# <a name="serviceupdatemessage-archive"></a><span data-ttu-id="0fa66-103">serviceUpdateMessage: архив</span><span class="sxs-lookup"><span data-stu-id="0fa66-103">serviceUpdateMessage: archive</span></span>
<span data-ttu-id="0fa66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa66-105">Архивировать список [serviceUpdateMessages](../resources/serviceupdatemessage.md) для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0fa66-105">Archive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa66-106">Permissions</span></span>
<span data-ttu-id="0fa66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa66-109">Permission type</span></span>|<span data-ttu-id="0fa66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fa66-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fa66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fa66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0fa66-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="0fa66-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="0fa66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fa66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fa66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa66-114">Not supported.</span></span>|
|<span data-ttu-id="0fa66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fa66-115">Application</span></span>|<span data-ttu-id="0fa66-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0fa66-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fa66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fa66-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/archive
```

## <a name="request-headers"></a><span data-ttu-id="0fa66-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fa66-118">Request headers</span></span>
|<span data-ttu-id="0fa66-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0fa66-119">Name</span></span>|<span data-ttu-id="0fa66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa66-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0fa66-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fa66-121">Authorization</span></span>|<span data-ttu-id="0fa66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa66-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0fa66-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fa66-124">Content-Type</span></span>|<span data-ttu-id="0fa66-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa66-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa66-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fa66-127">Request body</span></span>
<span data-ttu-id="0fa66-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="0fa66-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="0fa66-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0fa66-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0fa66-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="0fa66-130">Parameter</span></span>|<span data-ttu-id="0fa66-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0fa66-131">Type</span></span>|<span data-ttu-id="0fa66-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa66-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="0fa66-133">messageIds</span></span>|<span data-ttu-id="0fa66-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0fa66-134">String collection</span></span>|<span data-ttu-id="0fa66-135">Список ID-сообщений для архива.</span><span class="sxs-lookup"><span data-stu-id="0fa66-135">List of message IDs to archive.</span></span>|

## <a name="response"></a><span data-ttu-id="0fa66-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa66-136">Response</span></span>

<span data-ttu-id="0fa66-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0fa66-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="0fa66-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="0fa66-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa66-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0fa66-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa66-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa66-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_archive"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/archive
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a><span data-ttu-id="0fa66-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa66-141">Response</span></span>
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