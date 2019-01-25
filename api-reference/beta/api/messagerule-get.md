---
title: Получение правила
description: Получение свойств и связей объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7bf99f574d8e1a14ffaa7295d51a0dafca0d4628
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512558"
---
# <a name="get-rule"></a><span data-ttu-id="db5f7-103">Получение правила</span><span class="sxs-lookup"><span data-stu-id="db5f7-103">Get rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5f7-104">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="db5f7-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="db5f7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db5f7-105">Permissions</span></span>
<span data-ttu-id="db5f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db5f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db5f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db5f7-108">Permission type</span></span>      | <span data-ttu-id="db5f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db5f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db5f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db5f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db5f7-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="db5f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db5f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5f7-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="db5f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db5f7-114">Application</span></span> | <span data-ttu-id="db5f7-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="db5f7-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="db5f7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db5f7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db5f7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db5f7-117">Optional query parameters</span></span>
<span data-ttu-id="db5f7-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="db5f7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db5f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db5f7-119">Request headers</span></span>
| <span data-ttu-id="db5f7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db5f7-120">Name</span></span>      |<span data-ttu-id="db5f7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db5f7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db5f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db5f7-122">Authorization</span></span>  | <span data-ttu-id="db5f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db5f7-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="db5f7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db5f7-125">Request body</span></span>
<span data-ttu-id="db5f7-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db5f7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="db5f7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="db5f7-127">Response</span></span>
<span data-ttu-id="db5f7-128">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="db5f7-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db5f7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="db5f7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db5f7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="db5f7-130">Request</span></span>
<span data-ttu-id="db5f7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db5f7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="db5f7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="db5f7-132">Response</span></span>
<span data-ttu-id="db5f7-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db5f7-133">Here is an example of the response.</span></span> <span data-ttu-id="db5f7-134">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="db5f7-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="db5f7-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db5f7-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/messagerule-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
