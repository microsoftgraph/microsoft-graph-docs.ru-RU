---
title: Обновление Клаудпкпровисионингполици
description: Обновление свойств объекта Клаудпкпровисионингполици.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: d33f0395dbcff1794a7171882a3bc152f731f1f8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563312"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="3095b-103">Обновление Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="3095b-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="3095b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3095b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3095b-105">Обновление свойств объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3095b-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="3095b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3095b-106">Permissions</span></span>

<span data-ttu-id="3095b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3095b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3095b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3095b-109">Permission type</span></span>|<span data-ttu-id="3095b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3095b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3095b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3095b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3095b-112">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3095b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="3095b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3095b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3095b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3095b-114">Not supported.</span></span>|
|<span data-ttu-id="3095b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3095b-115">Application</span></span>|<span data-ttu-id="3095b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3095b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3095b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3095b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3095b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3095b-118">Request headers</span></span>

| <span data-ttu-id="3095b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3095b-119">Name</span></span>          | <span data-ttu-id="3095b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3095b-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="3095b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3095b-121">Authorization</span></span> | <span data-ttu-id="3095b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3095b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3095b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3095b-124">Content-Type</span></span>  | <span data-ttu-id="3095b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3095b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3095b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3095b-127">Request body</span></span>

<span data-ttu-id="3095b-128">В тексте запроса добавьте представление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3095b-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="3095b-129">В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3095b-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="3095b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3095b-130">Property</span></span>|<span data-ttu-id="3095b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3095b-131">Type</span></span>|<span data-ttu-id="3095b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3095b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3095b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3095b-133">displayName</span></span>|<span data-ttu-id="3095b-134">String</span><span class="sxs-lookup"><span data-stu-id="3095b-134">String</span></span>|<span data-ttu-id="3095b-135">Отображаемое имя политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="3095b-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="3095b-136">description</span><span class="sxs-lookup"><span data-stu-id="3095b-136">description</span></span>|<span data-ttu-id="3095b-137">String</span><span class="sxs-lookup"><span data-stu-id="3095b-137">String</span></span>|<span data-ttu-id="3095b-138">Описание политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="3095b-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="3095b-139">онпремисесконнектионид</span><span class="sxs-lookup"><span data-stu-id="3095b-139">onPremisesConnectionId</span></span>|<span data-ttu-id="3095b-140">String</span><span class="sxs-lookup"><span data-stu-id="3095b-140">String</span></span>|<span data-ttu-id="3095b-141">Идентификатор Клаудпконпремисесконнектион.</span><span class="sxs-lookup"><span data-stu-id="3095b-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="3095b-142">Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="3095b-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="3095b-143">имажеид</span><span class="sxs-lookup"><span data-stu-id="3095b-143">imageId</span></span>|<span data-ttu-id="3095b-144">String</span><span class="sxs-lookup"><span data-stu-id="3095b-144">String</span></span>|<span data-ttu-id="3095b-145">Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="3095b-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="3095b-146">Формат изображения для типа галереи: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="3095b-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="3095b-147">имажедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3095b-147">imageDisplayName</span></span>|<span data-ttu-id="3095b-148">String</span><span class="sxs-lookup"><span data-stu-id="3095b-148">String</span></span>|<span data-ttu-id="3095b-149">Отображаемое имя для образа ОС, который вы собираетесь заготовить.</span><span class="sxs-lookup"><span data-stu-id="3095b-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="3095b-150">имажетипе</span><span class="sxs-lookup"><span data-stu-id="3095b-150">imageType</span></span>|<span data-ttu-id="3095b-151">клаудпкпровисионингполициимажетипе</span><span class="sxs-lookup"><span data-stu-id="3095b-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="3095b-152">Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="3095b-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="3095b-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="3095b-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="3095b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3095b-154">Response</span></span>

<span data-ttu-id="3095b-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3095b-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3095b-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="3095b-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3095b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="3095b-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3095b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3095b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_provisioningpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
Content-Type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
# <a name="c"></a>[<span data-ttu-id="3095b-159">C#</span><span class="sxs-lookup"><span data-stu-id="3095b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3095b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3095b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3095b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3095b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3095b-162">Java</span><span class="sxs-lookup"><span data-stu-id="3095b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3095b-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3095b-163">Response</span></span>

<span data-ttu-id="3095b-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3095b-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "8931f750-f750-8931-50f7-318950f7ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
