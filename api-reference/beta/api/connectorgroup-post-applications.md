---
title: Создание приложения
description: С помощью этого API можно создать объект application.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cdbffc239b196a2b88b94862f5469d623dce69ec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943416"
---
# <a name="create-application"></a><span data-ttu-id="22082-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="22082-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22082-104">С помощью этого API можно создать объект application.</span><span class="sxs-lookup"><span data-stu-id="22082-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="22082-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22082-105">Permissions</span></span>
<span data-ttu-id="22082-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22082-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22082-108">Permission type</span></span>      | <span data-ttu-id="22082-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22082-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22082-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22082-110">Delegated (work or school account)</span></span> | <span data-ttu-id="22082-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22082-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22082-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22082-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22082-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22082-113">Not supported.</span></span>    |
|<span data-ttu-id="22082-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22082-114">Application</span></span> | <span data-ttu-id="22082-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22082-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22082-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22082-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="22082-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22082-117">Request headers</span></span>
| <span data-ttu-id="22082-118">Имя</span><span class="sxs-lookup"><span data-stu-id="22082-118">Name</span></span>       | <span data-ttu-id="22082-119">Описание</span><span class="sxs-lookup"><span data-stu-id="22082-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22082-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22082-120">Authorization</span></span>  | <span data-ttu-id="22082-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="22082-121">Bearer.</span></span> <span data-ttu-id="22082-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="22082-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="22082-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22082-123">Request body</span></span>
<span data-ttu-id="22082-124">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22082-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22082-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="22082-125">Response</span></span>

<span data-ttu-id="22082-126">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22082-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22082-127">Пример</span><span class="sxs-lookup"><span data-stu-id="22082-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22082-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="22082-128">Request</span></span>
<span data-ttu-id="22082-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22082-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="22082-130">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22082-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="22082-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="22082-131">Response</span></span>
<span data-ttu-id="22082-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22082-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
