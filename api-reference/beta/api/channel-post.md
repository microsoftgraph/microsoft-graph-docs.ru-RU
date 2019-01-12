---
title: Создание канала
description: Создайте новый канал в группы разработчиков Microsoft, как указано в тексте запроса.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 5f0046a496de37d5c1d2a3df0b7e452fbc38e4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980477"
---
# <a name="create-channel"></a><span data-ttu-id="64470-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="64470-103">Create Channel</span></span>

> <span data-ttu-id="64470-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64470-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64470-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64470-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64470-106">Создайте новый [канал](../resources/channel.md) в группы разработчиков Microsoft, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="64470-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="64470-107">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="64470-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="64470-108">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="64470-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="64470-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64470-109">Permissions</span></span>
<span data-ttu-id="64470-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64470-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64470-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64470-112">Permission type</span></span>      | <span data-ttu-id="64470-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64470-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64470-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64470-114">Delegated (work or school account)</span></span> | <span data-ttu-id="64470-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64470-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64470-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64470-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64470-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64470-117">Not supported.</span></span>    |
|<span data-ttu-id="64470-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64470-118">Application</span></span> | <span data-ttu-id="64470-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64470-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="64470-120">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="64470-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="64470-121">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="64470-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="64470-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64470-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="64470-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64470-123">Request headers</span></span>
| <span data-ttu-id="64470-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64470-124">Header</span></span>       | <span data-ttu-id="64470-125">Значение</span><span class="sxs-lookup"><span data-stu-id="64470-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64470-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64470-126">Authorization</span></span>  | <span data-ttu-id="64470-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64470-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64470-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64470-129">Content-Type</span></span>  | <span data-ttu-id="64470-130">application/json</span><span class="sxs-lookup"><span data-stu-id="64470-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64470-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64470-131">Request body</span></span>
<span data-ttu-id="64470-132">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="64470-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64470-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="64470-133">Response</span></span>

<span data-ttu-id="64470-134">Успешно завершена, этот метод возвращает `201 Created` объект [канала](../resources/channel.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64470-134">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64470-135">Пример</span><span class="sxs-lookup"><span data-stu-id="64470-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64470-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64470-136">Request</span></span>
<span data-ttu-id="64470-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64470-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="64470-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="64470-138">Response</span></span>
<span data-ttu-id="64470-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64470-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
