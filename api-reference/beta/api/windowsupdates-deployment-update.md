---
title: Обновление развертывания
description: Обновление свойств объекта развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2b5857f70136b804494825eb7cb66945d2b1a452
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785258"
---
# <a name="update-deployment"></a><span data-ttu-id="53a5c-103">Обновление развертывания</span><span class="sxs-lookup"><span data-stu-id="53a5c-103">Update deployment</span></span>
<span data-ttu-id="53a5c-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="53a5c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53a5c-105">Обновление свойств объекта [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="53a5c-105">Update the properties of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53a5c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53a5c-106">Permissions</span></span>
<span data-ttu-id="53a5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53a5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53a5c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53a5c-109">Permission type</span></span>|<span data-ttu-id="53a5c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53a5c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53a5c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53a5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53a5c-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a5c-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="53a5c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53a5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53a5c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53a5c-114">Not supported.</span></span>|
|<span data-ttu-id="53a5c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="53a5c-115">Application</span></span>|<span data-ttu-id="53a5c-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a5c-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53a5c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53a5c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="53a5c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53a5c-118">Request headers</span></span>
|<span data-ttu-id="53a5c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="53a5c-119">Name</span></span>|<span data-ttu-id="53a5c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53a5c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53a5c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53a5c-121">Authorization</span></span>|<span data-ttu-id="53a5c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53a5c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="53a5c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53a5c-124">Content-Type</span></span>|<span data-ttu-id="53a5c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53a5c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53a5c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53a5c-127">Request body</span></span>
<span data-ttu-id="53a5c-128">В теле запроса поставляем представление JSON объекта [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="53a5c-128">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="53a5c-129">В следующей таблице показаны свойства, которые можно установить при обновлении [развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="53a5c-129">The following table shows the properties that can be set when you update the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="53a5c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53a5c-130">Property</span></span>|<span data-ttu-id="53a5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53a5c-131">Type</span></span>|<span data-ttu-id="53a5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53a5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a5c-133">state</span><span class="sxs-lookup"><span data-stu-id="53a5c-133">state</span></span>|[<span data-ttu-id="53a5c-134">microsoft.graph.windowsUpdates.deploymentState</span><span class="sxs-lookup"><span data-stu-id="53a5c-134">microsoft.graph.windowsUpdates.deploymentState</span></span>](../resources/windowsupdates-deploymentstate.md)|<span data-ttu-id="53a5c-135">Состояние выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="53a5c-135">Execution status of the deployment.</span></span>|
|<span data-ttu-id="53a5c-136">settings</span><span class="sxs-lookup"><span data-stu-id="53a5c-136">settings</span></span>|[<span data-ttu-id="53a5c-137">microsoft.graph.windowsUpdates.deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="53a5c-137">microsoft.graph.windowsUpdates.deploymentSettings</span></span>](../resources/windowsupdates-deploymentsettings.md)|<span data-ttu-id="53a5c-138">Параметры конкретного развертывания, регулирующих `content` развертывание.</span><span class="sxs-lookup"><span data-stu-id="53a5c-138">Settings specified on the specific deployment governing how to deploy deployment `content`.</span></span>|


## <a name="response"></a><span data-ttu-id="53a5c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="53a5c-139">Response</span></span>

<span data-ttu-id="53a5c-140">В случае успешного применения этот метод возвращает код ответа и обновленный объект `202 Accepted` развертывания в тексте отклика. [](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="53a5c-140">If successful, this method returns a `202 Accepted` response code and an updated [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53a5c-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="53a5c-141">Examples</span></span>

### <a name="example-pause-a-deployment"></a><span data-ttu-id="53a5c-142">Пример: Приостановка развертывания</span><span class="sxs-lookup"><span data-stu-id="53a5c-142">Example: Pause a deployment</span></span>

<span data-ttu-id="53a5c-143">В этом примере развертывание приостановлено, `requestedValue` обновив `state` развертывание.</span><span class="sxs-lookup"><span data-stu-id="53a5c-143">In this example, the deployment is paused by updating the `requestedValue` of the deployment `state`.</span></span>

#### <a name="request"></a><span data-ttu-id="53a5c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="53a5c-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="53a5c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="53a5c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deployment_1",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "requestedValue": "paused"
  },
}
```
# <a name="c"></a>[<span data-ttu-id="53a5c-146">C#</span><span class="sxs-lookup"><span data-stu-id="53a5c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53a5c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53a5c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53a5c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53a5c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53a5c-149">Java</span><span class="sxs-lookup"><span data-stu-id="53a5c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="53a5c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="53a5c-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "pausedByRequest"
      }
    ],
    "requestedValue": "paused",
    "value": "paused"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": null,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-update-deployment-settings-to-add-a-monitoring-rule"></a><span data-ttu-id="53a5c-151">Пример. Обновление параметров развертывания, чтобы добавить правило мониторинга</span><span class="sxs-lookup"><span data-stu-id="53a5c-151">Example: Update deployment settings to add a monitoring rule</span></span>

<span data-ttu-id="53a5c-152">В этом примере свойство развертывания обновляется, чтобы `settings` добавить правило мониторинга.</span><span class="sxs-lookup"><span data-stu-id="53a5c-152">In this example, the `settings` property of the deployment is updated to add a monitoring rule.</span></span>

#### <a name="request"></a><span data-ttu-id="53a5c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="53a5c-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_deployment_2",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```


#### <a name="response"></a><span data-ttu-id="53a5c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="53a5c-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "value": "offering"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

