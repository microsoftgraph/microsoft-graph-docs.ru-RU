---
title: Создание развертывания
description: Создание нового объекта развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: b6ab12d7687d63a46684496c071fb4f9045a8786
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239226"
---
# <a name="create-deployment"></a><span data-ttu-id="fabda-103">Создание развертывания</span><span class="sxs-lookup"><span data-stu-id="fabda-103">Create deployment</span></span>
<span data-ttu-id="fabda-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fabda-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!NOTE]
> <span data-ttu-id="fabda-105">Если при создании [](/graph/api/resources/windowsupdates-monitoringrule) развертывания не указано правило мониторинга, создается правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fabda-105">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="fabda-106">Это правило мониторинга по умолчанию **имеет** сигнал `rollback` , пороговое значение и  `20` **действие** `alertError` .</span><span class="sxs-lookup"><span data-stu-id="fabda-106">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="fabda-107">В будущем обновлении API это поведение изменится и не будет создано правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fabda-107">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

<span data-ttu-id="fabda-108">Создание нового [объекта развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="fabda-108">Create a new [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fabda-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fabda-109">Permissions</span></span>
<span data-ttu-id="fabda-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fabda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fabda-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fabda-112">Permission type</span></span>|<span data-ttu-id="fabda-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fabda-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fabda-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fabda-114">Delegated (work or school account)</span></span>|<span data-ttu-id="fabda-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabda-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="fabda-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fabda-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fabda-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fabda-117">Not supported.</span></span>|
|<span data-ttu-id="fabda-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fabda-118">Application</span></span>|<span data-ttu-id="fabda-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabda-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fabda-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fabda-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments
```

## <a name="request-headers"></a><span data-ttu-id="fabda-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fabda-121">Request headers</span></span>
|<span data-ttu-id="fabda-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fabda-122">Name</span></span>|<span data-ttu-id="fabda-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fabda-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fabda-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fabda-124">Authorization</span></span>|<span data-ttu-id="fabda-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fabda-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fabda-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fabda-127">Content-Type</span></span>|<span data-ttu-id="fabda-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fabda-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fabda-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fabda-130">Request body</span></span>
<span data-ttu-id="fabda-131">В теле запроса поставляем представление JSON объекта [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="fabda-131">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="fabda-132">В следующей таблице показаны свойства, необходимые при создании [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="fabda-132">The following table shows the properties that are required when you create the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="fabda-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="fabda-133">Property</span></span>|<span data-ttu-id="fabda-134">Тип</span><span class="sxs-lookup"><span data-stu-id="fabda-134">Type</span></span>|<span data-ttu-id="fabda-135">Описание</span><span class="sxs-lookup"><span data-stu-id="fabda-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabda-136">content</span><span class="sxs-lookup"><span data-stu-id="fabda-136">content</span></span>|[<span data-ttu-id="fabda-137">microsoft.graph.windowsUpdates.deployableContent</span><span class="sxs-lookup"><span data-stu-id="fabda-137">microsoft.graph.windowsUpdates.deployableContent</span></span>](../resources/windowsupdates-deployablecontent.md)|<span data-ttu-id="fabda-138">Указывает, какой контент развернуть.</span><span class="sxs-lookup"><span data-stu-id="fabda-138">Specifies what content to deploy.</span></span> <span data-ttu-id="fabda-139">Развертываемый контент следует предоставлять в качестве одного из следующих производных типов: [speededQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) , [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)</span><span class="sxs-lookup"><span data-stu-id="fabda-139">Deployable content should be provided as one of the following derived types: [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) , [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fabda-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fabda-140">Response</span></span>

<span data-ttu-id="fabda-141">В случае успешного применения этот метод возвращает код ответа и `201 Created` объект [развертывания](../resources/windowsupdates-deployment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fabda-141">If successful, this method returns a `201 Created` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fabda-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="fabda-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fabda-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="fabda-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fabda-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fabda-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_deployment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-Type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="fabda-145">C#</span><span class="sxs-lookup"><span data-stu-id="fabda-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-deployment-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fabda-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fabda-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-deployment-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fabda-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fabda-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-deployment-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fabda-148">Java</span><span class="sxs-lookup"><span data-stu-id="fabda-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-deployment-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fabda-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fabda-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "value": "offering",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "effectiveSinceDate": "String (timestamp)"
    },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100,
      "durationBetweenOffers": "P7D",
      "startDateTime": null,
      "endDateTime": null
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    },
    "userExperience": null
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

