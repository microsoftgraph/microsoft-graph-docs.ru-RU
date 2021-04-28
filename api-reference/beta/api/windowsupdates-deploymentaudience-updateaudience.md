---
title: 'deploymentAudience: updateAudience'
description: Обновление коллекций участников и исключений развертыванияAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a0567070f4042896835b735fa69b5cd1dddeb1a3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067603"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="512f0-103">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="512f0-103">deploymentAudience: updateAudience</span></span>
<span data-ttu-id="512f0-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="512f0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="512f0-105">Обновление коллекций участников и исключений [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="512f0-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="512f0-106">Добавление [azureADDevice](../resources/windowsupdates-azureaddevice.md) в собрания участников или исключения аудитории развертывания автоматически создает объект устройства Azure AD, если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="512f0-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="512f0-107">Если один и тот же [updatableAsset](../resources/windowsupdates-updatableasset.md)  будет включен в коллекции исключений и членов **развертыванияAudience,** развертывание не будет применяться к этому активу. </span><span class="sxs-lookup"><span data-stu-id="512f0-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="512f0-108">Если все **объекты updatableAsset** одного типа, вы также можете использовать обновление [методаAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) для обновления **deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="512f0-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="512f0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="512f0-109">Permissions</span></span>
<span data-ttu-id="512f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="512f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="512f0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="512f0-112">Permission type</span></span>|<span data-ttu-id="512f0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="512f0-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="512f0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="512f0-114">Delegated (work or school account)</span></span>|<span data-ttu-id="512f0-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="512f0-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="512f0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="512f0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="512f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="512f0-117">Not supported.</span></span>|
|<span data-ttu-id="512f0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="512f0-118">Application</span></span>|<span data-ttu-id="512f0-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="512f0-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="512f0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="512f0-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="512f0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="512f0-121">Request headers</span></span>
|<span data-ttu-id="512f0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="512f0-122">Name</span></span>|<span data-ttu-id="512f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="512f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="512f0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="512f0-124">Authorization</span></span>|<span data-ttu-id="512f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="512f0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="512f0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="512f0-127">Content-Type</span></span>|<span data-ttu-id="512f0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="512f0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="512f0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="512f0-130">Request body</span></span>
<span data-ttu-id="512f0-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="512f0-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="512f0-132">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="512f0-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="512f0-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="512f0-133">Parameter</span></span>|<span data-ttu-id="512f0-134">Тип</span><span class="sxs-lookup"><span data-stu-id="512f0-134">Type</span></span>|<span data-ttu-id="512f0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="512f0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="512f0-136">addMembers</span><span class="sxs-lookup"><span data-stu-id="512f0-136">addMembers</span></span>|<span data-ttu-id="512f0-137">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="512f0-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="512f0-138">Список [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, которые необходимо добавить в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="512f0-138">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="512f0-139">removeMembers</span><span class="sxs-lookup"><span data-stu-id="512f0-139">removeMembers</span></span>|<span data-ttu-id="512f0-140">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="512f0-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="512f0-141">Список updatable активов, которые необходимо удалить в качестве членов аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="512f0-141">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="512f0-142">addExclusions</span><span class="sxs-lookup"><span data-stu-id="512f0-142">addExclusions</span></span>|<span data-ttu-id="512f0-143">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="512f0-143">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="512f0-144">Список updatable активов, которые необходимо добавить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="512f0-144">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="512f0-145">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="512f0-145">removeExclusions</span></span>|<span data-ttu-id="512f0-146">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="512f0-146">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="512f0-147">Список updatable активов, которые необходимо удалить в качестве исключений из аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="512f0-147">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="512f0-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="512f0-148">Response</span></span>

<span data-ttu-id="512f0-149">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="512f0-149">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="512f0-150">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="512f0-150">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="512f0-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="512f0-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="512f0-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="512f0-152">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="512f0-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="512f0-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

