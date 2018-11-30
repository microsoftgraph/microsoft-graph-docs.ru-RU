---
title: Список приложений
description: Получение списка объектов приложения, связанные с connectorGroup.
ms.openlocfilehash: 11d81454677b60e2402c4d1fe32aae5c974c1afc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078604"
---
# <a name="list-applications"></a><span data-ttu-id="34564-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="34564-103">List applications</span></span>

> <span data-ttu-id="34564-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34564-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34564-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34564-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34564-106">Получение списка объектов приложения, связанные с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="34564-106">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="34564-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34564-107">Permissions</span></span>
<span data-ttu-id="34564-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34564-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34564-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34564-110">Permission type</span></span>      | <span data-ttu-id="34564-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34564-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34564-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34564-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34564-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="34564-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34564-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34564-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34564-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34564-115">Not supported.</span></span>    |
|<span data-ttu-id="34564-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34564-116">Application</span></span> | <span data-ttu-id="34564-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34564-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34564-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34564-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34564-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34564-119">Optional query parameters</span></span>
<span data-ttu-id="34564-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="34564-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34564-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34564-121">Request headers</span></span>
| <span data-ttu-id="34564-122">Имя</span><span class="sxs-lookup"><span data-stu-id="34564-122">Name</span></span>      |<span data-ttu-id="34564-123">Описание</span><span class="sxs-lookup"><span data-stu-id="34564-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34564-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34564-124">Authorization</span></span>  | <span data-ttu-id="34564-125">Носителя.</span><span class="sxs-lookup"><span data-stu-id="34564-125">Bearer.</span></span> <span data-ttu-id="34564-126">Обязательный</span><span class="sxs-lookup"><span data-stu-id="34564-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="34564-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34564-127">Request body</span></span>
<span data-ttu-id="34564-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34564-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34564-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="34564-129">Response</span></span>

<span data-ttu-id="34564-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [приложения](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34564-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34564-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34564-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34564-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34564-132">Request</span></span>
<span data-ttu-id="34564-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34564-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="34564-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="34564-134">Response</span></span>
<span data-ttu-id="34564-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="34564-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "appId": "appId-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "customDomainCertificate": "customDomainCertificate-value",
        "isTranslateHostHeaderEnabled": true,
        "isOnPremPublishingEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
