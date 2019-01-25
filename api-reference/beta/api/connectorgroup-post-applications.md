---
title: Создание приложения
description: Используйте этот интерфейс API для создания нового приложения.
localization_priority: Normal
ms.openlocfilehash: 350e5f0fcb45f7404a670c1a0af4e4ddd02a97c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514245"
---
# <a name="create-application"></a><span data-ttu-id="5ebb2-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="5ebb2-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ebb2-104">Используйте этот интерфейс API для создания нового приложения.</span><span class="sxs-lookup"><span data-stu-id="5ebb2-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ebb2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ebb2-105">Permissions</span></span>
<span data-ttu-id="5ebb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebb2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ebb2-108">Permission type</span></span>      | <span data-ttu-id="5ebb2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ebb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ebb2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ebb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ebb2-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ebb2-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ebb2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ebb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ebb2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebb2-113">Not supported.</span></span>    |
|<span data-ttu-id="5ebb2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ebb2-114">Application</span></span> | <span data-ttu-id="5ebb2-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebb2-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ebb2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ebb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="5ebb2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ebb2-117">Request headers</span></span>
| <span data-ttu-id="5ebb2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5ebb2-118">Name</span></span>       | <span data-ttu-id="5ebb2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5ebb2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ebb2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebb2-120">Authorization</span></span>  | <span data-ttu-id="5ebb2-121">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="5ebb2-121">Bearer.</span></span> <span data-ttu-id="5ebb2-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="5ebb2-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebb2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ebb2-123">Request body</span></span>
<span data-ttu-id="5ebb2-124">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="5ebb2-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5ebb2-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ebb2-125">Response</span></span>

<span data-ttu-id="5ebb2-126">Успешно завершена, этот метод возвращает `201 Created` объект ответа кодов и [приложений](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5ebb2-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebb2-127">Пример</span><span class="sxs-lookup"><span data-stu-id="5ebb2-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ebb2-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ebb2-128">Request</span></span>
<span data-ttu-id="5ebb2-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ebb2-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="5ebb2-130">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="5ebb2-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5ebb2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ebb2-131">Response</span></span>
<span data-ttu-id="5ebb2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5ebb2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
