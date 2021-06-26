---
title: 'serviceUpdateMessage: любимый'
description: Измените состояние списка сообщений обновления службы на избранное для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 619053e68a7d5633d095223bca4ddda604f49083
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151743"
---
# <a name="serviceupdatemessage-favorite"></a><span data-ttu-id="e2bdb-103">serviceUpdateMessage: любимый</span><span class="sxs-lookup"><span data-stu-id="e2bdb-103">serviceUpdateMessage: favorite</span></span>
<span data-ttu-id="e2bdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2bdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2bdb-105">Измените состояние списка [serviceUpdateMessages на](../resources/serviceupdatemessage.md) избранное для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-105">Change the status of a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) to favorite for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2bdb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2bdb-106">Permissions</span></span>
<span data-ttu-id="e2bdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2bdb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2bdb-109">Permission type</span></span>|<span data-ttu-id="e2bdb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2bdb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2bdb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2bdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2bdb-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="e2bdb-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="e2bdb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2bdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2bdb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-114">Not supported.</span></span>|
|<span data-ttu-id="e2bdb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2bdb-115">Application</span></span>|<span data-ttu-id="e2bdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2bdb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2bdb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/favorite
```

## <a name="request-headers"></a><span data-ttu-id="e2bdb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2bdb-118">Request headers</span></span>
|<span data-ttu-id="e2bdb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2bdb-119">Name</span></span>|<span data-ttu-id="e2bdb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2bdb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2bdb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2bdb-121">Authorization</span></span>|<span data-ttu-id="e2bdb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e2bdb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2bdb-124">Content-Type</span></span>|<span data-ttu-id="e2bdb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2bdb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2bdb-127">Request body</span></span>
<span data-ttu-id="e2bdb-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="e2bdb-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e2bdb-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2bdb-130">Parameter</span></span>|<span data-ttu-id="e2bdb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2bdb-131">Type</span></span>|<span data-ttu-id="e2bdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2bdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2bdb-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="e2bdb-133">messageIds</span></span>|<span data-ttu-id="e2bdb-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e2bdb-134">String collection</span></span>|<span data-ttu-id="e2bdb-135">Список ID-сообщений для сохранения в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-135">List of message IDs to save as favorite.</span></span>|

## <a name="response"></a><span data-ttu-id="e2bdb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2bdb-136">Response</span></span>

<span data-ttu-id="e2bdb-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="e2bdb-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="e2bdb-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2bdb-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e2bdb-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2bdb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2bdb-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_favorite"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/favorite
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a><span data-ttu-id="e2bdb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2bdb-141">Response</span></span>
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
