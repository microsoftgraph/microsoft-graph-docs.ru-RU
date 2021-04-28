---
title: 'deploymentAudience: updateAudienceById'
description: Обновление семейство участников и исключения развертыванияAudience с помощью updatableAsset ресурсов того же типа.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 60970c5d6b02d8c9de79e206eab2360a156c5eee
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068040"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="fa380-103">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="fa380-103">deploymentAudience: updateAudienceById</span></span>
<span data-ttu-id="fa380-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fa380-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa380-105">Обновление семейство участников и исключения [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md) с помощью [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов того же типа.</span><span class="sxs-lookup"><span data-stu-id="fa380-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="fa380-106">Добавление [azureADDevice](../resources/windowsupdates-azureaddevice.md) в собрания участников или исключения аудитории развертывания автоматически создает объект устройства Azure AD, если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="fa380-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="fa380-107">Если один и тот же [updatableAsset](../resources/windowsupdates-updatableasset.md)  будет включен в коллекции исключений и членов **развертыванияAudience,** развертывание не будет применяться к этому активу. </span><span class="sxs-lookup"><span data-stu-id="fa380-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="fa380-108">Вы также можете использовать обновление [методаAudience](windowsupdates-deploymentaudience-updateaudience.md) для обновления **deploymentAudience.**</span><span class="sxs-lookup"><span data-stu-id="fa380-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa380-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa380-109">Permissions</span></span>
<span data-ttu-id="fa380-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa380-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa380-112">Permission type</span></span>|<span data-ttu-id="fa380-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa380-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa380-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa380-114">Delegated (work or school account)</span></span>|<span data-ttu-id="fa380-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa380-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="fa380-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa380-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa380-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa380-117">Not supported.</span></span>|
|<span data-ttu-id="fa380-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa380-118">Application</span></span>|<span data-ttu-id="fa380-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa380-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa380-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa380-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="fa380-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa380-121">Request headers</span></span>
|<span data-ttu-id="fa380-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fa380-122">Name</span></span>|<span data-ttu-id="fa380-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fa380-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa380-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa380-124">Authorization</span></span>|<span data-ttu-id="fa380-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa380-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa380-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa380-127">Content-Type</span></span>|<span data-ttu-id="fa380-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa380-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa380-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa380-130">Request body</span></span>
<span data-ttu-id="fa380-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa380-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fa380-132">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fa380-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fa380-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="fa380-133">Parameter</span></span>|<span data-ttu-id="fa380-134">Тип</span><span class="sxs-lookup"><span data-stu-id="fa380-134">Type</span></span>|<span data-ttu-id="fa380-135">Описание</span><span class="sxs-lookup"><span data-stu-id="fa380-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa380-136">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="fa380-136">memberEntityType</span></span>|<span data-ttu-id="fa380-137">String</span><span class="sxs-lookup"><span data-stu-id="fa380-137">String</span></span>|<span data-ttu-id="fa380-138">Полный тип updatable активов.</span><span class="sxs-lookup"><span data-stu-id="fa380-138">The full type of the updatable assets.</span></span> <span data-ttu-id="fa380-139">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span><span class="sxs-lookup"><span data-stu-id="fa380-139">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="fa380-140">addMembers</span><span class="sxs-lookup"><span data-stu-id="fa380-140">addMembers</span></span>|<span data-ttu-id="fa380-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa380-141">String collection</span></span>|<span data-ttu-id="fa380-142">Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="fa380-142">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="fa380-143">removeMembers</span><span class="sxs-lookup"><span data-stu-id="fa380-143">removeMembers</span></span>|<span data-ttu-id="fa380-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa380-144">String collection</span></span>|<span data-ttu-id="fa380-145">Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве членов аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="fa380-145">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="fa380-146">addExclusions</span><span class="sxs-lookup"><span data-stu-id="fa380-146">addExclusions</span></span>|<span data-ttu-id="fa380-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa380-147">String collection</span></span>|<span data-ttu-id="fa380-148">Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="fa380-148">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="fa380-149">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="fa380-149">removeExclusions</span></span>|<span data-ttu-id="fa380-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa380-150">String collection</span></span>|<span data-ttu-id="fa380-151">Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="fa380-151">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="fa380-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa380-152">Response</span></span>

<span data-ttu-id="fa380-153">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="fa380-153">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="fa380-154">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa380-154">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa380-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa380-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa380-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa380-156">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="fa380-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa380-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

