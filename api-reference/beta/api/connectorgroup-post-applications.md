---
title: Добавление приложения в Коннекторграуп
description: Используйте этот API, чтобы назначить приложение для группы соединителей
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7843d1fa661bfcaf209fbdfee52f08f96427a37f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555796"
---
# <a name="add-an-application-to-a-connectorgroup"></a><span data-ttu-id="09c8c-103">Добавление приложения в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="09c8c-103">Add an application to a connectorGroup</span></span>

<span data-ttu-id="09c8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09c8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c8c-105">Добавление [приложения](../resources/application.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="09c8c-105">Add an [application](../resources/application.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09c8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09c8c-106">Permissions</span></span>
<span data-ttu-id="09c8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09c8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09c8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09c8c-109">Permission type</span></span>      | <span data-ttu-id="09c8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09c8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09c8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09c8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09c8c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09c8c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09c8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09c8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09c8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09c8c-114">Not supported.</span></span>    |
|<span data-ttu-id="09c8c-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="09c8c-115">Application</span></span> | <span data-ttu-id="09c8c-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c8c-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09c8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09c8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="09c8c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09c8c-118">Request headers</span></span>
| <span data-ttu-id="09c8c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="09c8c-119">Name</span></span>       | <span data-ttu-id="09c8c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="09c8c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09c8c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09c8c-121">Authorization</span></span>  | <span data-ttu-id="09c8c-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="09c8c-122">Bearer.</span></span> <span data-ttu-id="09c8c-123">Обязательное</span><span class="sxs-lookup"><span data-stu-id="09c8c-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="09c8c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09c8c-124">Request body</span></span>
<span data-ttu-id="09c8c-125">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09c8c-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09c8c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c8c-126">Response</span></span>

<span data-ttu-id="09c8c-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09c8c-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c8c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="09c8c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09c8c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="09c8c-129">Request</span></span>
<span data-ttu-id="09c8c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09c8c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/beta/applications/{id}"
}
```
<span data-ttu-id="09c8c-131">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09c8c-131">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="09c8c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c8c-132">Response</span></span>
<span data-ttu-id="09c8c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09c8c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
