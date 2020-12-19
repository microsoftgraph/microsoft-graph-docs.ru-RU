---
title: Назначение соединителиГрупп приложению
description: Использование этого API для назначения соединителиГрупп приложению
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac902f4a1287a8d27fcf9ad571172207ca7b8e50
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719957"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="386ff-103">Назначение соединителиГрупп приложению</span><span class="sxs-lookup"><span data-stu-id="386ff-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="386ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="386ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="386ff-105">[Назначьте соединителиГрупп](../resources/connectorgroup.md) [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="386ff-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="386ff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="386ff-106">Permissions</span></span>
<span data-ttu-id="386ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="386ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="386ff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="386ff-109">Permission type</span></span>      | <span data-ttu-id="386ff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="386ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="386ff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="386ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="386ff-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="386ff-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="386ff-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="386ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="386ff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="386ff-114">Not supported.</span></span>    |
|<span data-ttu-id="386ff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="386ff-115">Application</span></span> | <span data-ttu-id="386ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="386ff-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="386ff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="386ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="386ff-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="386ff-118">Request headers</span></span>
| <span data-ttu-id="386ff-119">Имя</span><span class="sxs-lookup"><span data-stu-id="386ff-119">Name</span></span>       | <span data-ttu-id="386ff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="386ff-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="386ff-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="386ff-121">Authorization</span></span>  | <span data-ttu-id="386ff-122">Bearer.</span><span class="sxs-lookup"><span data-stu-id="386ff-122">Bearer.</span></span> <span data-ttu-id="386ff-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="386ff-123">Required.</span></span>|
| <span data-ttu-id="386ff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="386ff-124">Content-type</span></span> | <span data-ttu-id="386ff-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="386ff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="386ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="386ff-127">Request body</span></span>
<span data-ttu-id="386ff-128">В теле запроса укажете представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="386ff-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="386ff-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="386ff-129">Response</span></span>

<span data-ttu-id="386ff-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="386ff-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="386ff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="386ff-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="386ff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="386ff-132">Request</span></span>
<span data-ttu-id="386ff-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="386ff-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="386ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="386ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/connectorGroup/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="386ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="386ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="386ff-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="386ff-136">Response</span></span>
<span data-ttu-id="386ff-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="386ff-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Assign a connectorGroup to an application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


