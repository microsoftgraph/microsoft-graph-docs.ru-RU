---
title: Список приложений
description: Получение списка объектов приложения, связанные с connectorGroup.
localization_priority: Normal
ms.openlocfilehash: f23bd18d646233fd932c10e5f2fe4d8bda1732d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833384"
---
# <a name="list-applications"></a><span data-ttu-id="02be4-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="02be4-103">List applications</span></span>

> <span data-ttu-id="02be4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02be4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02be4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02be4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02be4-106">Получение списка объектов приложения, связанные с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="02be4-106">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="02be4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02be4-107">Permissions</span></span>
<span data-ttu-id="02be4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02be4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02be4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02be4-110">Permission type</span></span>      | <span data-ttu-id="02be4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02be4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02be4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02be4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02be4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02be4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02be4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02be4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02be4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02be4-115">Not supported.</span></span>    |
|<span data-ttu-id="02be4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02be4-116">Application</span></span> | <span data-ttu-id="02be4-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02be4-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02be4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02be4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02be4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02be4-119">Optional query parameters</span></span>
<span data-ttu-id="02be4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02be4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02be4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02be4-121">Request headers</span></span>
| <span data-ttu-id="02be4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="02be4-122">Name</span></span>      |<span data-ttu-id="02be4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="02be4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02be4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02be4-124">Authorization</span></span>  | <span data-ttu-id="02be4-125">Носителя.</span><span class="sxs-lookup"><span data-stu-id="02be4-125">Bearer.</span></span> <span data-ttu-id="02be4-126">Обязательное</span><span class="sxs-lookup"><span data-stu-id="02be4-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="02be4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02be4-127">Request body</span></span>
<span data-ttu-id="02be4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02be4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02be4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="02be4-129">Response</span></span>

<span data-ttu-id="02be4-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [приложения](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02be4-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02be4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="02be4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02be4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="02be4-132">Request</span></span>
<span data-ttu-id="02be4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02be4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="02be4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="02be4-134">Response</span></span>
<span data-ttu-id="02be4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="02be4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
