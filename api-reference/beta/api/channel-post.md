---
title: Создание канала
description: Создайте новый канал в группы разработчиков Microsoft, как указано в тексте запроса.
ms.openlocfilehash: f9767c70c94ce4cfe3379310c425005ace8fbe1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077280"
---
# <a name="create-channel"></a><span data-ttu-id="379a9-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="379a9-103">Create Channel</span></span>

> <span data-ttu-id="379a9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="379a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="379a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="379a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="379a9-106">Создайте новый [канал](../resources/channel.md) в группы разработчиков Microsoft, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="379a9-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="379a9-107">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="379a9-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="379a9-108">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="379a9-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="379a9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="379a9-109">Permissions</span></span>
<span data-ttu-id="379a9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="379a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="379a9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="379a9-112">Permission type</span></span>      | <span data-ttu-id="379a9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="379a9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="379a9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="379a9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="379a9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="379a9-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="379a9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="379a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="379a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="379a9-117">Not supported.</span></span>    |
|<span data-ttu-id="379a9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="379a9-118">Application</span></span> | <span data-ttu-id="379a9-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="379a9-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="379a9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="379a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="379a9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="379a9-121">Request headers</span></span>
| <span data-ttu-id="379a9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="379a9-122">Header</span></span>       | <span data-ttu-id="379a9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="379a9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="379a9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="379a9-124">Authorization</span></span>  | <span data-ttu-id="379a9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="379a9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="379a9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="379a9-127">Content-Type</span></span>  | <span data-ttu-id="379a9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="379a9-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="379a9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="379a9-129">Request body</span></span>
<span data-ttu-id="379a9-130">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="379a9-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="379a9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="379a9-131">Response</span></span>

<span data-ttu-id="379a9-132">Успешно завершена, этот метод возвращает `201 Created` объект [канала](../resources/channel.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="379a9-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="379a9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="379a9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="379a9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="379a9-134">Request</span></span>
<span data-ttu-id="379a9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="379a9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="379a9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="379a9-136">Response</span></span>
<span data-ttu-id="379a9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="379a9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
