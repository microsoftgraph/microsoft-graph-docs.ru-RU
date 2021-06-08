---
title: 'канал: provisionEmail'
description: Подготовка электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35865ff1b44fad5bc66951df571dbd5252a363df
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813254"
---
# <a name="channel-provisionemail"></a><span data-ttu-id="973ae-103">канал: provisionEmail</span><span class="sxs-lookup"><span data-stu-id="973ae-103">channel: provisionEmail</span></span>

<span data-ttu-id="973ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="973ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="973ae-105">Предоставление адреса электронной почты для [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="973ae-105">Provision an email address for a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="973ae-106">Microsoft Teams автоматически не содержит адрес электронной почты для канала по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="973ae-106">Microsoft Teams does not automatically provision an email address for a channel by default.</span></span> <span data-ttu-id="973ae-107">Чтобы Teams адрес электронной почты, можно вызвать **provisionEmail** или с помощью пользовательского интерфейса Teams, выберите get email address **,** который запускает Teams для создания адреса электронной почты, если он еще не был предварительно.</span><span class="sxs-lookup"><span data-stu-id="973ae-107">To have Teams provision an email address, you can call **provisionEmail**, or through the Teams user interface, select **Get email address**, which triggers Teams to generate an email address if it has not already provisioned one.</span></span>

<span data-ttu-id="973ae-108">Чтобы удалить предварительный адрес электронной почты канала, используйте [метод removeEmail.](channel-removeemail.md)</span><span class="sxs-lookup"><span data-stu-id="973ae-108">To remove a channel's provisioned email address, use the [removeEmail](channel-removeemail.md) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="973ae-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="973ae-109">Permissions</span></span>

<span data-ttu-id="973ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="973ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="973ae-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="973ae-112">Permission type</span></span>                        | <span data-ttu-id="973ae-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="973ae-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="973ae-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="973ae-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="973ae-115">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="973ae-115">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="973ae-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="973ae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="973ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="973ae-117">Not supported.</span></span>                              |
| <span data-ttu-id="973ae-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="973ae-118">Application</span></span>                            | <span data-ttu-id="973ae-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="973ae-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="973ae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="973ae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a><span data-ttu-id="973ae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="973ae-121">Request headers</span></span>
| <span data-ttu-id="973ae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="973ae-122">Header</span></span>        | <span data-ttu-id="973ae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="973ae-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="973ae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="973ae-124">Authorization</span></span> | <span data-ttu-id="973ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="973ae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="973ae-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="973ae-127">Request body</span></span>

<span data-ttu-id="973ae-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="973ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="973ae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="973ae-129">Response</span></span>

<span data-ttu-id="973ae-130">Если электронная почта канала будет успешно продюсироваться, этот метод возвращает код ответа и объект `200 OK` [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="973ae-130">If the channel's email is provisioned successfully, this method returns a `200 OK` response code and a [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) object in the response body.</span></span> <span data-ttu-id="973ae-131">Предварительный адрес электронной почты находится в **свойстве электронной** почты.</span><span class="sxs-lookup"><span data-stu-id="973ae-131">The provisioned email address is in the **email** property.</span></span>

## <a name="example"></a><span data-ttu-id="973ae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="973ae-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="973ae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="973ae-133">Request</span></span>
<span data-ttu-id="973ae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="973ae-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```

### <a name="response"></a><span data-ttu-id="973ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="973ae-135">Response</span></span>
<span data-ttu-id="973ae-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="973ae-136">The following is an example of a response.</span></span>
<span data-ttu-id="973ae-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="973ae-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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


