---
title: Исправление канала
description: Обновляет свойства указанного канала.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 73d777999d6112de44cffc6fb8e9a4cd36ee093c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832845"
---
# <a name="patch-channel"></a><span data-ttu-id="cd136-103">Исправление канала</span><span class="sxs-lookup"><span data-stu-id="cd136-103">Patch channel</span></span>



<span data-ttu-id="cd136-104">Обновляет свойства указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="cd136-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="cd136-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="cd136-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="cd136-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="cd136-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd136-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd136-107">Permissions</span></span>
<span data-ttu-id="cd136-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd136-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd136-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd136-110">Permission type</span></span>      | <span data-ttu-id="cd136-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd136-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd136-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd136-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd136-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd136-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd136-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd136-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd136-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd136-115">Not supported.</span></span>    |
|<span data-ttu-id="cd136-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd136-116">Application</span></span> | <span data-ttu-id="cd136-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd136-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="cd136-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="cd136-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cd136-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="cd136-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cd136-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd136-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cd136-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd136-121">Request headers</span></span>
| <span data-ttu-id="cd136-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd136-122">Header</span></span>       | <span data-ttu-id="cd136-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cd136-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd136-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd136-124">Authorization</span></span>  | <span data-ttu-id="cd136-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd136-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd136-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd136-127">Content-Type</span></span>  | <span data-ttu-id="cd136-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cd136-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd136-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd136-129">Request body</span></span>
<span data-ttu-id="cd136-130">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="cd136-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd136-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd136-131">Response</span></span>

<span data-ttu-id="cd136-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd136-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd136-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cd136-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd136-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd136-134">Request</span></span>
<span data-ttu-id="cd136-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd136-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="cd136-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd136-136">Response</span></span>
<span data-ttu-id="cd136-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cd136-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
