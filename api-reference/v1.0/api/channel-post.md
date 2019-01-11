---
title: Создание канала
description: Создайте новый канал в группы разработчиков Microsoft, как указано в тексте запроса.
localization_priority: Priority
ms.openlocfilehash: d80659a3ecb69a33a9ea3a23a9ce94f13d6b95a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847595"
---
# <a name="create-channel"></a><span data-ttu-id="59b3e-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="59b3e-103">Create Channel</span></span>



<span data-ttu-id="59b3e-104">Создайте новый [канал](../resources/channel.md) в группы разработчиков Microsoft, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="59b3e-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="59b3e-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="59b3e-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="59b3e-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="59b3e-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="59b3e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59b3e-107">Permissions</span></span>
<span data-ttu-id="59b3e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59b3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="59b3e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59b3e-110">Permission type</span></span>      | <span data-ttu-id="59b3e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59b3e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b3e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59b3e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59b3e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b3e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59b3e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59b3e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b3e-115">Not supported.</span></span>    |
|<span data-ttu-id="59b3e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59b3e-116">Application</span></span> | <span data-ttu-id="59b3e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b3e-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="59b3e-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="59b3e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="59b3e-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="59b3e-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="59b3e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59b3e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="59b3e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59b3e-121">Request headers</span></span>
| <span data-ttu-id="59b3e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59b3e-122">Header</span></span>       | <span data-ttu-id="59b3e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="59b3e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59b3e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59b3e-124">Authorization</span></span>  | <span data-ttu-id="59b3e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59b3e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59b3e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59b3e-127">Content-Type</span></span>  | <span data-ttu-id="59b3e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59b3e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59b3e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59b3e-129">Request body</span></span>
<span data-ttu-id="59b3e-130">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="59b3e-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59b3e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="59b3e-131">Response</span></span>

<span data-ttu-id="59b3e-132">Успешно завершена, этот метод возвращает `201 Created` объект [канала](../resources/channel.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="59b3e-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59b3e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="59b3e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59b3e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="59b3e-134">Request</span></span>
<span data-ttu-id="59b3e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59b3e-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="59b3e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="59b3e-136">Response</span></span>
<span data-ttu-id="59b3e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59b3e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
