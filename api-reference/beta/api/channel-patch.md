---
title: Исправление канала
description: Обновляет свойства указанного канала.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 78f2d8eebf70d52b6067612c715939d7463b17f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894084"
---
# <a name="patch-channel"></a><span data-ttu-id="355c2-103">Исправление канала</span><span class="sxs-lookup"><span data-stu-id="355c2-103">Patch channel</span></span>

> <span data-ttu-id="355c2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="355c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="355c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="355c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="355c2-106">Обновляет свойства указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="355c2-106">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="355c2-107">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="355c2-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="355c2-108">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="355c2-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="355c2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="355c2-109">Permissions</span></span>
<span data-ttu-id="355c2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="355c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="355c2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="355c2-112">Permission type</span></span>      | <span data-ttu-id="355c2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="355c2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="355c2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="355c2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="355c2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355c2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="355c2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="355c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="355c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="355c2-117">Not supported.</span></span>    |
|<span data-ttu-id="355c2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="355c2-118">Application</span></span> | <span data-ttu-id="355c2-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355c2-119">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="355c2-120">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="355c2-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="355c2-121">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="355c2-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="355c2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="355c2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="355c2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="355c2-123">Request headers</span></span>
| <span data-ttu-id="355c2-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="355c2-124">Header</span></span>       | <span data-ttu-id="355c2-125">Значение</span><span class="sxs-lookup"><span data-stu-id="355c2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="355c2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="355c2-126">Authorization</span></span>  | <span data-ttu-id="355c2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="355c2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="355c2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="355c2-129">Content-Type</span></span>  | <span data-ttu-id="355c2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="355c2-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="355c2-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="355c2-131">Request body</span></span>
<span data-ttu-id="355c2-132">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="355c2-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="355c2-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="355c2-133">Response</span></span>

<span data-ttu-id="355c2-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="355c2-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="355c2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="355c2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="355c2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="355c2-136">Request</span></span>
<span data-ttu-id="355c2-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="355c2-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="355c2-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="355c2-138">Response</span></span>
<span data-ttu-id="355c2-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="355c2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
