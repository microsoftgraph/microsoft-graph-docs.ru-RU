---
title: 'serviceUpdateMessage: неархивный'
description: Unarchive a list of service update messages for the signed in user.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 38144a2f3e6512631f47a22ebecdf7a41e70a417
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209134"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="79c69-103">serviceUpdateMessage: неархивный</span><span class="sxs-lookup"><span data-stu-id="79c69-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="79c69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79c69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79c69-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="79c69-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="79c69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79c69-106">Permissions</span></span>
<span data-ttu-id="79c69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79c69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79c69-109">Permission type</span></span>|<span data-ttu-id="79c69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79c69-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79c69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79c69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79c69-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="79c69-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="79c69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79c69-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79c69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c69-114">Not supported.</span></span>|
|<span data-ttu-id="79c69-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="79c69-115">Application</span></span>|<span data-ttu-id="79c69-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79c69-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="79c69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79c69-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="79c69-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79c69-118">Request headers</span></span>
|<span data-ttu-id="79c69-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79c69-119">Name</span></span>|<span data-ttu-id="79c69-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79c69-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79c69-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79c69-121">Authorization</span></span>|<span data-ttu-id="79c69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79c69-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79c69-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79c69-124">Content-Type</span></span>|<span data-ttu-id="79c69-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79c69-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79c69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79c69-127">Request body</span></span>
<span data-ttu-id="79c69-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="79c69-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="79c69-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="79c69-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="79c69-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="79c69-130">Parameter</span></span>|<span data-ttu-id="79c69-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79c69-131">Type</span></span>|<span data-ttu-id="79c69-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79c69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79c69-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="79c69-133">messageIds</span></span>|<span data-ttu-id="79c69-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79c69-134">String collection</span></span>|<span data-ttu-id="79c69-135">Список ID-сообщений для неархивных.</span><span class="sxs-lookup"><span data-stu-id="79c69-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="79c69-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c69-136">Response</span></span>

<span data-ttu-id="79c69-137">В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79c69-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="79c69-138">В противном случае `false` возвращается в тело ответа.</span><span class="sxs-lookup"><span data-stu-id="79c69-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c69-139">Пример</span><span class="sxs-lookup"><span data-stu-id="79c69-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="79c69-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="79c69-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="79c69-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="79c69-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="79c69-142">C#</span><span class="sxs-lookup"><span data-stu-id="79c69-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceupdatemessage-unarchive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79c69-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79c69-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceupdatemessage-unarchive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79c69-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79c69-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceupdatemessage-unarchive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79c69-145">Java</span><span class="sxs-lookup"><span data-stu-id="79c69-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceupdatemessage-unarchive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="79c69-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c69-146">Response</span></span>
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
