---
title: 'serviceUpdateMessage: любимый'
description: Измените состояние списка сообщений обновления службы на избранное для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 5838b8c395db539f06aad31ef7794eda2f8587ad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107829"
---
# <a name="serviceupdatemessage-favorite"></a><span data-ttu-id="833f9-103">serviceUpdateMessage: любимый</span><span class="sxs-lookup"><span data-stu-id="833f9-103">serviceUpdateMessage: favorite</span></span>
<span data-ttu-id="833f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="833f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="833f9-105">Измените состояние списка [serviceUpdateMessages на](../resources/serviceupdatemessage.md) избранное для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="833f9-105">Change the status of a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) to favorite for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="833f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="833f9-106">Permissions</span></span>
<span data-ttu-id="833f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="833f9-109">Permission type</span></span>|<span data-ttu-id="833f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="833f9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="833f9-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="833f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="833f9-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="833f9-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="833f9-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="833f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="833f9-114">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="833f9-114">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="833f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="833f9-115">Application</span></span>|<span data-ttu-id="833f9-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="833f9-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="833f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="833f9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/favorite
```

## <a name="request-headers"></a><span data-ttu-id="833f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="833f9-118">Request headers</span></span>
|<span data-ttu-id="833f9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="833f9-119">Name</span></span>|<span data-ttu-id="833f9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="833f9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="833f9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="833f9-121">Authorization</span></span>|<span data-ttu-id="833f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="833f9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="833f9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="833f9-124">Content-Type</span></span>|<span data-ttu-id="833f9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="833f9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="833f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="833f9-127">Request body</span></span>
<span data-ttu-id="833f9-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="833f9-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="833f9-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="833f9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="833f9-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="833f9-130">Parameter</span></span>|<span data-ttu-id="833f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="833f9-131">Type</span></span>|<span data-ttu-id="833f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="833f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="833f9-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="833f9-133">messageIds</span></span>|<span data-ttu-id="833f9-134">Набор строк</span><span class="sxs-lookup"><span data-stu-id="833f9-134">String collection</span></span>|<span data-ttu-id="833f9-135">Список ID-сообщений для сохранения в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="833f9-135">List of message IDs to save as favorite.</span></span>|

## <a name="response"></a><span data-ttu-id="833f9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="833f9-136">Response</span></span>

<span data-ttu-id="833f9-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="833f9-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="833f9-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="833f9-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="833f9-139">Пример</span><span class="sxs-lookup"><span data-stu-id="833f9-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="833f9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="833f9-140">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="833f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="833f9-141">Response</span></span>
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
