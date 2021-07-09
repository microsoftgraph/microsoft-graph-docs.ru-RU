---
title: 'deploymentAudience: updateAudience'
description: Обновление коллекций участников и исключений развертыванияAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 23fe655e076987ffb33591eb8aaa1600ed4a8fa4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351127"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="b6a53-103">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="b6a53-103">deploymentAudience: updateAudience</span></span>

<span data-ttu-id="b6a53-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b6a53-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a53-105">Обновление коллекций участников и исключений [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="b6a53-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="b6a53-106">Добавление [azureADDevice](../resources/windowsupdates-azureaddevice.md) в собрания участников или исключения аудитории развертывания автоматически создает объект устройства Azure AD, если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="b6a53-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="b6a53-107">Если один и тот же [updatableAsset](../resources/windowsupdates-updatableasset.md)  будет включен в коллекции исключений и членов **развертыванияAudience,** развертывание не будет применяться к этому активу. </span><span class="sxs-lookup"><span data-stu-id="b6a53-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="b6a53-108">Если все **объекты updatableAsset** одного типа, вы также можете использовать обновление [методаAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) для обновления **deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="b6a53-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

> [!NOTE]
> <span data-ttu-id="b6a53-109">Этот API имеет [известные проблемы, связанные](/Graph/known-issues#accessing-and-updating-deployment-audiences) с развертываниями, созданными через Intune.</span><span class="sxs-lookup"><span data-stu-id="b6a53-109">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a53-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a53-110">Permissions</span></span>
<span data-ttu-id="b6a53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a53-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a53-113">Permission type</span></span>|<span data-ttu-id="b6a53-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6a53-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6a53-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a53-115">Delegated (work or school account)</span></span>|<span data-ttu-id="b6a53-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a53-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="b6a53-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a53-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a53-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a53-118">Not supported.</span></span>|
|<span data-ttu-id="b6a53-119">Application</span><span class="sxs-lookup"><span data-stu-id="b6a53-119">Application</span></span>|<span data-ttu-id="b6a53-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a53-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6a53-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a53-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="b6a53-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a53-122">Request headers</span></span>
|<span data-ttu-id="b6a53-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b6a53-123">Name</span></span>|<span data-ttu-id="b6a53-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a53-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6a53-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6a53-125">Authorization</span></span>|<span data-ttu-id="b6a53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a53-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6a53-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6a53-128">Content-Type</span></span>|<span data-ttu-id="b6a53-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a53-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a53-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6a53-131">Request body</span></span>
<span data-ttu-id="b6a53-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6a53-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6a53-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b6a53-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6a53-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="b6a53-134">Parameter</span></span>|<span data-ttu-id="b6a53-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a53-135">Type</span></span>|<span data-ttu-id="b6a53-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a53-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a53-137">addMembers</span><span class="sxs-lookup"><span data-stu-id="b6a53-137">addMembers</span></span>|<span data-ttu-id="b6a53-138">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b6a53-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b6a53-139">Список [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, которые необходимо добавить в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="b6a53-139">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="b6a53-140">removeMembers</span><span class="sxs-lookup"><span data-stu-id="b6a53-140">removeMembers</span></span>|<span data-ttu-id="b6a53-141">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b6a53-141">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b6a53-142">Список updatable активов, которые необходимо удалить в качестве членов аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="b6a53-142">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="b6a53-143">addExclusions</span><span class="sxs-lookup"><span data-stu-id="b6a53-143">addExclusions</span></span>|<span data-ttu-id="b6a53-144">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b6a53-144">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b6a53-145">Список updatable активов, которые необходимо добавить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="b6a53-145">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="b6a53-146">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="b6a53-146">removeExclusions</span></span>|<span data-ttu-id="b6a53-147">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b6a53-147">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b6a53-148">Список updatable активов, которые необходимо удалить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="b6a53-148">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="b6a53-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6a53-149">Response</span></span>

<span data-ttu-id="b6a53-150">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b6a53-150">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b6a53-151">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a53-151">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6a53-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="b6a53-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6a53-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a53-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6a53-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a53-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudience"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-Type: application/json
Content-length: 599

{
  "addMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "addExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b6a53-155">C#</span><span class="sxs-lookup"><span data-stu-id="b6a53-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudience-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6a53-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6a53-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudience-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6a53-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6a53-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudience-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6a53-158">Java</span><span class="sxs-lookup"><span data-stu-id="b6a53-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudience-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b6a53-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a53-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

