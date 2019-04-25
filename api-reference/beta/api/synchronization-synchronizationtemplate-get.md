---
title: Получение Синчронизатионтемплате
description: Получение шаблона синхронизации по его идентификатору.
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545183"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="346a6-103">Получение Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="346a6-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="346a6-104">Получение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="346a6-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="346a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="346a6-105">Permissions</span></span>
<span data-ttu-id="346a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="346a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="346a6-108">Permission type</span></span>                        | <span data-ttu-id="346a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="346a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="346a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="346a6-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="346a6-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346a6-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="346a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="346a6-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="346a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346a6-113">Not supported.</span></span>|
|<span data-ttu-id="346a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="346a6-114">Application</span></span>                            |<span data-ttu-id="346a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346a6-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="346a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="346a6-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="346a6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="346a6-117">Request headers</span></span>

| <span data-ttu-id="346a6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="346a6-118">Name</span></span>           | <span data-ttu-id="346a6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="346a6-119">Type</span></span>    | <span data-ttu-id="346a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="346a6-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="346a6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="346a6-121">Authorization</span></span>  | <span data-ttu-id="346a6-122">string</span><span class="sxs-lookup"><span data-stu-id="346a6-122">string</span></span>  | <span data-ttu-id="346a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="346a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="346a6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="346a6-125">Request body</span></span>

<span data-ttu-id="346a6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="346a6-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="346a6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="346a6-127">Response</span></span>

<span data-ttu-id="346a6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="346a6-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="346a6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="346a6-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="346a6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="346a6-130">Request</span></span>
<span data-ttu-id="346a6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="346a6-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="346a6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="346a6-132">Response</span></span>
<span data-ttu-id="346a6-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="346a6-133">The following is an example of a response.</span></span>
><span data-ttu-id="346a6-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="346a6-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="346a6-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="346a6-135">All the properties will be returned in an actual call.</span></span>

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
