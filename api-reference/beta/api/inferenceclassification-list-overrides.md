---
title: Переопределение списка
description: Получение параметров сортировки папки "Входящие", которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.
localization_priority: Normal
ms.openlocfilehash: a49d47e39caff5c00981d02551b0eeb564239f73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501282"
---
# <a name="list-overrides"></a><span data-ttu-id="ebf54-103">Переопределение списка</span><span class="sxs-lookup"><span data-stu-id="ebf54-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf54-104">Получение параметров [сортировки папки "Входящие"](../resources/manage-focused-inbox.md) , которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.</span><span class="sxs-lookup"><span data-stu-id="ebf54-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="ebf54-105">Каждое переопределение соответствует SMTP-адресу отправителя.</span><span class="sxs-lookup"><span data-stu-id="ebf54-105">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="ebf54-106">Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="ebf54-106">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebf54-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebf54-107">Permissions</span></span>
<span data-ttu-id="ebf54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebf54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebf54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebf54-110">Permission type</span></span>      | <span data-ttu-id="ebf54-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebf54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebf54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebf54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebf54-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf54-113">Mail.Read</span></span>    |
|<span data-ttu-id="ebf54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebf54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebf54-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf54-115">Mail.Read</span></span>    |
|<span data-ttu-id="ebf54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebf54-116">Application</span></span> | <span data-ttu-id="ebf54-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf54-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebf54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebf54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="ebf54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebf54-119">Request headers</span></span>
| <span data-ttu-id="ebf54-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ebf54-120">Name</span></span>       | <span data-ttu-id="ebf54-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf54-121">Type</span></span> | <span data-ttu-id="ebf54-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf54-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebf54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf54-123">Authorization</span></span>  | <span data-ttu-id="ebf54-124">string</span><span class="sxs-lookup"><span data-stu-id="ebf54-124">string</span></span>  | <span data-ttu-id="ebf54-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebf54-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebf54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebf54-127">Request body</span></span>
<span data-ttu-id="ebf54-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebf54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebf54-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebf54-129">Response</span></span>

<span data-ttu-id="ebf54-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebf54-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebf54-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ebf54-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebf54-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebf54-132">Request</span></span>
<span data-ttu-id="ebf54-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebf54-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="ebf54-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebf54-134">Response</span></span>
<span data-ttu-id="ebf54-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebf54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassification-list-overrides.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
