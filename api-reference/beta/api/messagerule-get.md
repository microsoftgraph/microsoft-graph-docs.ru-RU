---
title: Получение правила
description: Получение свойств и связей объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 53b1b4db43ed6a9e94564c618e0c302f4ec16bad
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333212"
---
# <a name="get-rule"></a><span data-ttu-id="a8a12-103">Получение правила</span><span class="sxs-lookup"><span data-stu-id="a8a12-103">Get rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a12-104">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="a8a12-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="a8a12-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8a12-105">Permissions</span></span>
<span data-ttu-id="a8a12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a12-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8a12-108">Permission type</span></span>      | <span data-ttu-id="a8a12-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8a12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a12-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8a12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a12-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8a12-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a8a12-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8a12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a12-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8a12-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a8a12-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8a12-114">Application</span></span> | <span data-ttu-id="a8a12-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8a12-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8a12-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8a12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a8a12-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8a12-117">Optional query parameters</span></span>
<span data-ttu-id="a8a12-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8a12-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8a12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8a12-119">Request headers</span></span>
| <span data-ttu-id="a8a12-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a8a12-120">Name</span></span>      |<span data-ttu-id="a8a12-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a8a12-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8a12-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8a12-122">Authorization</span></span>  | <span data-ttu-id="a8a12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8a12-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a8a12-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8a12-125">Request body</span></span>
<span data-ttu-id="a8a12-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8a12-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a8a12-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8a12-127">Response</span></span>
<span data-ttu-id="a8a12-128">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8a12-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8a12-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a8a12-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8a12-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8a12-130">Request</span></span>
<span data-ttu-id="a8a12-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8a12-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="a8a12-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8a12-132">Response</span></span>
<span data-ttu-id="a8a12-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8a12-133">Here is an example of the response.</span></span> <span data-ttu-id="a8a12-134">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a8a12-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="a8a12-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8a12-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
