---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 568236babb70a709f2c76e2804129adcbfdc0b03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328151"
---
# <a name="patch-channel"></a><span data-ttu-id="ea6d7-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="ea6d7-103">Patch channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea6d7-104">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ea6d7-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ea6d7-105">**Note**: существует известная проблема, связанная с разрешениями приложения и этим API.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="ea6d7-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="ea6d7-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea6d7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea6d7-107">Permissions</span></span>
<span data-ttu-id="ea6d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea6d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea6d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea6d7-110">Permission type</span></span>      | <span data-ttu-id="ea6d7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea6d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea6d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea6d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea6d7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea6d7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea6d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea6d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea6d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-115">Not supported.</span></span>    |
|<span data-ttu-id="ea6d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea6d7-116">Application</span></span> | <span data-ttu-id="ea6d7-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea6d7-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="ea6d7-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ea6d7-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ea6d7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea6d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ea6d7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea6d7-121">Request headers</span></span>
| <span data-ttu-id="ea6d7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea6d7-122">Header</span></span>       | <span data-ttu-id="ea6d7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ea6d7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea6d7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea6d7-124">Authorization</span></span>  | <span data-ttu-id="ea6d7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea6d7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea6d7-127">Content-Type</span></span>  | <span data-ttu-id="ea6d7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea6d7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea6d7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea6d7-129">Request body</span></span>
<span data-ttu-id="ea6d7-130">В тексте запроса добавьте представление объекта [Channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea6d7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea6d7-131">Response</span></span>

<span data-ttu-id="ea6d7-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea6d7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ea6d7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea6d7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea6d7-134">Request</span></span>
<span data-ttu-id="ea6d7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="ea6d7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea6d7-136">Response</span></span>
<span data-ttu-id="ea6d7-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea6d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
