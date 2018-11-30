---
title: Исправление канала
description: Обновляет свойства указанного канала.
ms.openlocfilehash: 981de62dcedb42b98016aa99ccaaa8b5cd27ba9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028509"
---
# <a name="patch-channel"></a><span data-ttu-id="9aef8-103">Исправление канала</span><span class="sxs-lookup"><span data-stu-id="9aef8-103">Patch channel</span></span>



<span data-ttu-id="9aef8-104">Обновляет свойства указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9aef8-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="9aef8-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="9aef8-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="9aef8-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="9aef8-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="9aef8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9aef8-107">Permissions</span></span>
<span data-ttu-id="9aef8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aef8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aef8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9aef8-110">Permission type</span></span>      | <span data-ttu-id="9aef8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9aef8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9aef8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9aef8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9aef8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aef8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9aef8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9aef8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9aef8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aef8-115">Not supported.</span></span>    |
|<span data-ttu-id="9aef8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9aef8-116">Application</span></span> | <span data-ttu-id="9aef8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aef8-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9aef8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9aef8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9aef8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9aef8-119">Request headers</span></span>
| <span data-ttu-id="9aef8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9aef8-120">Header</span></span>       | <span data-ttu-id="9aef8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9aef8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9aef8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9aef8-122">Authorization</span></span>  | <span data-ttu-id="9aef8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9aef8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9aef8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9aef8-125">Content-Type</span></span>  | <span data-ttu-id="9aef8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9aef8-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9aef8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9aef8-127">Request body</span></span>
<span data-ttu-id="9aef8-128">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="9aef8-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9aef8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9aef8-129">Response</span></span>

<span data-ttu-id="9aef8-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9aef8-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9aef8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9aef8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9aef8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9aef8-132">Request</span></span>
<span data-ttu-id="9aef8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9aef8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="9aef8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9aef8-134">Response</span></span>
<span data-ttu-id="9aef8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9aef8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
