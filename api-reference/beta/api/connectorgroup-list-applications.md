---
title: Список приложений
description: Получение списка объектов приложения, связанных с Коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: 47be81d4f154d87865113fa02b04a58151545507
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455760"
---
# <a name="list-applications"></a><span data-ttu-id="25e79-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="25e79-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e79-104">Получение списка объектов приложения, связанных с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="25e79-104">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="25e79-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25e79-105">Permissions</span></span>
<span data-ttu-id="25e79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e79-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25e79-108">Permission type</span></span>      | <span data-ttu-id="25e79-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25e79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e79-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25e79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25e79-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="25e79-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25e79-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25e79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25e79-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25e79-113">Not supported.</span></span>    |
|<span data-ttu-id="25e79-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25e79-114">Application</span></span> | <span data-ttu-id="25e79-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e79-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25e79-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25e79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25e79-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25e79-117">Optional query parameters</span></span>
<span data-ttu-id="25e79-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25e79-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25e79-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25e79-119">Request headers</span></span>
| <span data-ttu-id="25e79-120">Имя</span><span class="sxs-lookup"><span data-stu-id="25e79-120">Name</span></span>      |<span data-ttu-id="25e79-121">Описание</span><span class="sxs-lookup"><span data-stu-id="25e79-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25e79-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25e79-122">Authorization</span></span>  | <span data-ttu-id="25e79-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="25e79-123">Bearer.</span></span> <span data-ttu-id="25e79-124">Обязательно</span><span class="sxs-lookup"><span data-stu-id="25e79-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="25e79-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25e79-125">Request body</span></span>
<span data-ttu-id="25e79-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25e79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25e79-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="25e79-127">Response</span></span>

<span data-ttu-id="25e79-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25e79-128">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25e79-129">Пример</span><span class="sxs-lookup"><span data-stu-id="25e79-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25e79-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="25e79-130">Request</span></span>
<span data-ttu-id="25e79-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25e79-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="25e79-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e79-132">Response</span></span>
<span data-ttu-id="25e79-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25e79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-list-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
