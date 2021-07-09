---
title: 'deploymentAudience: updateAudienceById'
description: Обновление семейство участников и исключения развертыванияAudience с помощью updatableAsset ресурсов того же типа.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1b948e644628eedc08fe470641b612501dfb80af
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351120"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="9cc77-103">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="9cc77-103">deploymentAudience: updateAudienceById</span></span>

<span data-ttu-id="9cc77-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9cc77-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc77-105">Обновление семейство участников и исключения [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md) с помощью [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов того же типа.</span><span class="sxs-lookup"><span data-stu-id="9cc77-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="9cc77-106">Добавление [azureADDevice](../resources/windowsupdates-azureaddevice.md) в собрания участников или исключения аудитории развертывания автоматически создает объект устройства Azure AD, если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="9cc77-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="9cc77-107">Если один и тот же [updatableAsset](../resources/windowsupdates-updatableasset.md)  будет включен в коллекции исключений и членов **развертыванияAudience,** развертывание не будет применяться к этому активу. </span><span class="sxs-lookup"><span data-stu-id="9cc77-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="9cc77-108">Вы также можете использовать обновление [методаAudience](windowsupdates-deploymentaudience-updateaudience.md) для обновления **deploymentAudience.**</span><span class="sxs-lookup"><span data-stu-id="9cc77-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

> [!NOTE]
> <span data-ttu-id="9cc77-109">Этот API имеет [известные проблемы, связанные](/Graph/known-issues#accessing-and-updating-deployment-audiences) с развертываниями, созданными через Intune.</span><span class="sxs-lookup"><span data-stu-id="9cc77-109">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc77-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cc77-110">Permissions</span></span>
<span data-ttu-id="9cc77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc77-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cc77-113">Permission type</span></span>|<span data-ttu-id="9cc77-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cc77-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc77-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cc77-115">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc77-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc77-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9cc77-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cc77-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc77-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc77-118">Not supported.</span></span>|
|<span data-ttu-id="9cc77-119">Application</span><span class="sxs-lookup"><span data-stu-id="9cc77-119">Application</span></span>|<span data-ttu-id="9cc77-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc77-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc77-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cc77-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="9cc77-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cc77-122">Request headers</span></span>
|<span data-ttu-id="9cc77-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9cc77-123">Name</span></span>|<span data-ttu-id="9cc77-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9cc77-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9cc77-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cc77-125">Authorization</span></span>|<span data-ttu-id="9cc77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cc77-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9cc77-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc77-128">Content-Type</span></span>|<span data-ttu-id="9cc77-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cc77-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc77-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cc77-131">Request body</span></span>
<span data-ttu-id="9cc77-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cc77-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9cc77-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9cc77-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9cc77-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9cc77-134">Parameter</span></span>|<span data-ttu-id="9cc77-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9cc77-135">Type</span></span>|<span data-ttu-id="9cc77-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9cc77-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cc77-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="9cc77-137">memberEntityType</span></span>|<span data-ttu-id="9cc77-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9cc77-138">String</span></span>|<span data-ttu-id="9cc77-139">Полный тип updatable активов.</span><span class="sxs-lookup"><span data-stu-id="9cc77-139">The full type of the updatable assets.</span></span> <span data-ttu-id="9cc77-140">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cc77-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="9cc77-141">addMembers</span><span class="sxs-lookup"><span data-stu-id="9cc77-141">addMembers</span></span>|<span data-ttu-id="9cc77-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cc77-142">String collection</span></span>|<span data-ttu-id="9cc77-143">Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="9cc77-143">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="9cc77-144">removeMembers</span><span class="sxs-lookup"><span data-stu-id="9cc77-144">removeMembers</span></span>|<span data-ttu-id="9cc77-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cc77-145">String collection</span></span>|<span data-ttu-id="9cc77-146">Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве членов аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="9cc77-146">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="9cc77-147">addExclusions</span><span class="sxs-lookup"><span data-stu-id="9cc77-147">addExclusions</span></span>|<span data-ttu-id="9cc77-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cc77-148">String collection</span></span>|<span data-ttu-id="9cc77-149">Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="9cc77-149">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="9cc77-150">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="9cc77-150">removeExclusions</span></span>|<span data-ttu-id="9cc77-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cc77-151">String collection</span></span>|<span data-ttu-id="9cc77-152">Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="9cc77-152">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="9cc77-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cc77-153">Response</span></span>

<span data-ttu-id="9cc77-154">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="9cc77-154">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9cc77-155">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9cc77-155">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cc77-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="9cc77-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cc77-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cc77-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cc77-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc77-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json
Content-length: 204

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9cc77-159">C#</span><span class="sxs-lookup"><span data-stu-id="9cc77-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc77-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc77-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc77-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc77-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc77-162">Java</span><span class="sxs-lookup"><span data-stu-id="9cc77-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9cc77-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc77-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

