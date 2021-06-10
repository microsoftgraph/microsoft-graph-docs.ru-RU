---
title: 'канал: provisionEmail'
description: Подготовка электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b2e619970c0cdadd574a4873cb3231a88934a087
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869626"
---
# <a name="channel-provisionemail"></a><span data-ttu-id="fee44-103">канал: provisionEmail</span><span class="sxs-lookup"><span data-stu-id="fee44-103">channel: provisionEmail</span></span>

<span data-ttu-id="fee44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fee44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee44-105">Предоставление адреса электронной почты для [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fee44-105">Provision an email address for a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="fee44-106">Microsoft Teams автоматически не содержит адрес электронной почты для канала по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fee44-106">Microsoft Teams does not automatically provision an email address for a channel by default.</span></span> <span data-ttu-id="fee44-107">Чтобы Teams адрес электронной почты, можно вызвать **provisionEmail** или с помощью пользовательского интерфейса Teams, выберите get email address **,** который запускает Teams для создания адреса электронной почты, если он еще не был предварительно.</span><span class="sxs-lookup"><span data-stu-id="fee44-107">To have Teams provision an email address, you can call **provisionEmail**, or through the Teams user interface, select **Get email address**, which triggers Teams to generate an email address if it has not already provisioned one.</span></span>

<span data-ttu-id="fee44-108">Чтобы удалить предварительный адрес электронной почты канала, используйте [метод removeEmail.](channel-removeemail.md)</span><span class="sxs-lookup"><span data-stu-id="fee44-108">To remove a channel's provisioned email address, use the [removeEmail](channel-removeemail.md) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="fee44-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fee44-109">Permissions</span></span>

<span data-ttu-id="fee44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fee44-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fee44-112">Permission type</span></span>                        | <span data-ttu-id="fee44-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fee44-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fee44-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fee44-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fee44-115">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fee44-115">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="fee44-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fee44-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fee44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fee44-117">Not supported.</span></span>                              |
| <span data-ttu-id="fee44-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fee44-118">Application</span></span>                            | <span data-ttu-id="fee44-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fee44-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="fee44-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fee44-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a><span data-ttu-id="fee44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fee44-121">Request headers</span></span>
| <span data-ttu-id="fee44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fee44-122">Header</span></span>        | <span data-ttu-id="fee44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fee44-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="fee44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fee44-124">Authorization</span></span> | <span data-ttu-id="fee44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fee44-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fee44-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fee44-127">Request body</span></span>

<span data-ttu-id="fee44-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fee44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fee44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fee44-129">Response</span></span>

<span data-ttu-id="fee44-130">Если электронная почта канала будет успешно продюсироваться, этот метод возвращает код ответа и объект `200 OK` [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fee44-130">If the channel's email is provisioned successfully, this method returns a `200 OK` response code and a [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) object in the response body.</span></span> <span data-ttu-id="fee44-131">Предварительный адрес электронной почты находится в **свойстве электронной** почты.</span><span class="sxs-lookup"><span data-stu-id="fee44-131">The provisioned email address is in the **email** property.</span></span>

## <a name="example"></a><span data-ttu-id="fee44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fee44-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="fee44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fee44-133">Request</span></span>
<span data-ttu-id="fee44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fee44-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fee44-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fee44-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```
# <a name="c"></a>[<span data-ttu-id="fee44-136">C#</span><span class="sxs-lookup"><span data-stu-id="fee44-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-provisionemail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fee44-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fee44-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-provisionemail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fee44-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fee44-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-provisionemail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fee44-139">Java</span><span class="sxs-lookup"><span data-stu-id="fee44-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-provisionemail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fee44-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fee44-140">Response</span></span>
<span data-ttu-id="fee44-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fee44-141">The following is an example of a response.</span></span>
<span data-ttu-id="fee44-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fee44-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
    "email": "1df8f174.teamsgraph.onmicrosoft.com@amer.teams.ms"
}
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Provision channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


