---
title: Список приложений
description: Получение списка объектов приложения, связанных с Коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 350bc05c94bf177a350ee681e83cc16323f26046
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437471"
---
# <a name="list-applications"></a><span data-ttu-id="62401-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="62401-103">List applications</span></span>

<span data-ttu-id="62401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62401-105">Получение списка объектов приложения, связанных с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="62401-105">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="62401-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62401-106">Permissions</span></span>
<span data-ttu-id="62401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62401-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62401-109">Permission type</span></span>      | <span data-ttu-id="62401-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62401-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62401-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62401-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62401-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62401-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62401-114">Not supported.</span></span>    |
|<span data-ttu-id="62401-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62401-115">Application</span></span> | <span data-ttu-id="62401-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62401-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62401-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62401-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="62401-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62401-118">Optional query parameters</span></span>
<span data-ttu-id="62401-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="62401-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62401-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62401-120">Request headers</span></span>
| <span data-ttu-id="62401-121">Имя</span><span class="sxs-lookup"><span data-stu-id="62401-121">Name</span></span>      |<span data-ttu-id="62401-122">Описание</span><span class="sxs-lookup"><span data-stu-id="62401-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62401-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62401-123">Authorization</span></span>  | <span data-ttu-id="62401-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="62401-124">Bearer.</span></span> <span data-ttu-id="62401-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="62401-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="62401-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62401-126">Request body</span></span>
<span data-ttu-id="62401-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62401-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62401-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="62401-128">Response</span></span>

<span data-ttu-id="62401-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62401-129">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62401-130">Пример</span><span class="sxs-lookup"><span data-stu-id="62401-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62401-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="62401-131">Request</span></span>
<span data-ttu-id="62401-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62401-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="62401-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="62401-133">Response</span></span>
<span data-ttu-id="62401-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62401-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
