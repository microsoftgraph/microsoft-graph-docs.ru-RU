---
title: Создание приложения
description: Используйте этот интерфейс API для создания нового приложения.
ms.openlocfilehash: 08300057f78671ce74dd98bd98f7d3182bde083d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077926"
---
# <a name="create-application"></a><span data-ttu-id="4bda0-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="4bda0-103">Create application</span></span>

> <span data-ttu-id="4bda0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4bda0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bda0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bda0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bda0-106">Используйте этот интерфейс API для создания нового приложения.</span><span class="sxs-lookup"><span data-stu-id="4bda0-106">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bda0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bda0-107">Permissions</span></span>
<span data-ttu-id="4bda0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bda0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bda0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bda0-110">Permission type</span></span>      | <span data-ttu-id="4bda0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bda0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bda0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bda0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bda0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4bda0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4bda0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bda0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bda0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bda0-115">Not supported.</span></span>    |
|<span data-ttu-id="4bda0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bda0-116">Application</span></span> | <span data-ttu-id="4bda0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bda0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bda0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bda0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="4bda0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bda0-119">Request headers</span></span>
| <span data-ttu-id="4bda0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4bda0-120">Name</span></span>       | <span data-ttu-id="4bda0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4bda0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bda0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bda0-122">Authorization</span></span>  | <span data-ttu-id="4bda0-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="4bda0-123">Bearer.</span></span> <span data-ttu-id="4bda0-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="4bda0-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bda0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bda0-125">Request body</span></span>
<span data-ttu-id="4bda0-126">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="4bda0-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4bda0-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bda0-127">Response</span></span>

<span data-ttu-id="4bda0-128">Успешно завершена, этот метод возвращает `201 Created` объект ответа кодов и [приложений](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bda0-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bda0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4bda0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bda0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bda0-130">Request</span></span>
<span data-ttu-id="4bda0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bda0-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="4bda0-132">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="4bda0-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4bda0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bda0-133">Response</span></span>
<span data-ttu-id="4bda0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4bda0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
