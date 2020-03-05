---
title: Создание приложения
description: С помощью этого API можно создать объект application.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 018288444be3c2851e71117e1710a08947fa6104
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437359"
---
# <a name="create-application"></a><span data-ttu-id="31df6-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="31df6-103">Create application</span></span>

<span data-ttu-id="31df6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31df6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31df6-105">С помощью этого API можно создать объект application.</span><span class="sxs-lookup"><span data-stu-id="31df6-105">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="31df6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31df6-106">Permissions</span></span>
<span data-ttu-id="31df6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31df6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31df6-109">Permission type</span></span>      | <span data-ttu-id="31df6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31df6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31df6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31df6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31df6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31df6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31df6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31df6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31df6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31df6-114">Not supported.</span></span>    |
|<span data-ttu-id="31df6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31df6-115">Application</span></span> | <span data-ttu-id="31df6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31df6-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31df6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31df6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="31df6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31df6-118">Request headers</span></span>
| <span data-ttu-id="31df6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="31df6-119">Name</span></span>       | <span data-ttu-id="31df6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="31df6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31df6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31df6-121">Authorization</span></span>  | <span data-ttu-id="31df6-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="31df6-122">Bearer.</span></span> <span data-ttu-id="31df6-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="31df6-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="31df6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31df6-124">Request body</span></span>
<span data-ttu-id="31df6-125">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31df6-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31df6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="31df6-126">Response</span></span>

<span data-ttu-id="31df6-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31df6-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31df6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="31df6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31df6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="31df6-129">Request</span></span>
<span data-ttu-id="31df6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31df6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="31df6-131">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31df6-131">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="31df6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="31df6-132">Response</span></span>
<span data-ttu-id="31df6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31df6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
