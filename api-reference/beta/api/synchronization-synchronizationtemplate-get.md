---
title: Получение synchronizationTemplate
description: Извлечь шаблон синхронизации по идентификатору.
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524375"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="f5a50-103">Получение synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="f5a50-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5a50-104">Извлечь шаблон синхронизации по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f5a50-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5a50-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5a50-105">Permissions</span></span>
<span data-ttu-id="f5a50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5a50-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5a50-108">Permission type</span></span>                        | <span data-ttu-id="f5a50-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5a50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5a50-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5a50-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="f5a50-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5a50-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f5a50-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5a50-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f5a50-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5a50-113">Not supported.</span></span>|
|<span data-ttu-id="f5a50-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5a50-114">Application</span></span>                            |<span data-ttu-id="f5a50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5a50-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="f5a50-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5a50-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="f5a50-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5a50-117">Request headers</span></span>

| <span data-ttu-id="f5a50-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f5a50-118">Name</span></span>           | <span data-ttu-id="f5a50-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f5a50-119">Type</span></span>    | <span data-ttu-id="f5a50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f5a50-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f5a50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5a50-121">Authorization</span></span>  | <span data-ttu-id="f5a50-122">string</span><span class="sxs-lookup"><span data-stu-id="f5a50-122">string</span></span>  | <span data-ttu-id="f5a50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5a50-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5a50-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5a50-125">Request body</span></span>

<span data-ttu-id="f5a50-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5a50-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f5a50-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5a50-127">Response</span></span>

<span data-ttu-id="f5a50-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f5a50-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="f5a50-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f5a50-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f5a50-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5a50-130">Request</span></span>
<span data-ttu-id="f5a50-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5a50-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="f5a50-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5a50-132">Response</span></span>
<span data-ttu-id="f5a50-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5a50-133">The following is an example of a response.</span></span>
><span data-ttu-id="f5a50-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f5a50-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f5a50-135">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="f5a50-135">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
