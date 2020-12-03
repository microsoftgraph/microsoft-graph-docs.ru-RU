---
title: Создание Клаудпкпровисионингполици
description: Создайте новую политику подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 45410405c88d7bb8a3e8de544e40279af490386a
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563879"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="5fb36-103">Создание Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="5fb36-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="5fb36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb36-105">Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5fb36-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="5fb36-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb36-106">Permissions</span></span>

<span data-ttu-id="5fb36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fb36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fb36-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb36-109">Permission type</span></span>|<span data-ttu-id="5fb36-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fb36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fb36-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fb36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb36-112">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5fb36-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="5fb36-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fb36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fb36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fb36-114">Not supported.</span></span>|
|<span data-ttu-id="5fb36-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fb36-115">Application</span></span>|<span data-ttu-id="5fb36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fb36-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fb36-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fb36-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5fb36-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fb36-118">Request headers</span></span>

| <span data-ttu-id="5fb36-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5fb36-119">Name</span></span>          | <span data-ttu-id="5fb36-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb36-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="5fb36-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fb36-121">Authorization</span></span> | <span data-ttu-id="5fb36-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fb36-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5fb36-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5fb36-124">Content-Type</span></span>  | <span data-ttu-id="5fb36-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fb36-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb36-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fb36-127">Request body</span></span>

<span data-ttu-id="5fb36-128">В тексте запроса добавьте представление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fb36-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="5fb36-129">В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fb36-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="5fb36-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fb36-130">Property</span></span>|<span data-ttu-id="5fb36-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5fb36-131">Type</span></span>|<span data-ttu-id="5fb36-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb36-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5fb36-133">displayName</span></span>|<span data-ttu-id="5fb36-134">String</span><span class="sxs-lookup"><span data-stu-id="5fb36-134">String</span></span>|<span data-ttu-id="5fb36-135">Отображаемое имя политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="5fb36-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="5fb36-136">description</span><span class="sxs-lookup"><span data-stu-id="5fb36-136">description</span></span>|<span data-ttu-id="5fb36-137">String</span><span class="sxs-lookup"><span data-stu-id="5fb36-137">String</span></span>|<span data-ttu-id="5fb36-138">Описание политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="5fb36-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="5fb36-139">онпремисесконнектионид</span><span class="sxs-lookup"><span data-stu-id="5fb36-139">onPremisesConnectionId</span></span>|<span data-ttu-id="5fb36-140">String</span><span class="sxs-lookup"><span data-stu-id="5fb36-140">String</span></span>|<span data-ttu-id="5fb36-141">Идентификатор Клаудпконпремисесконнектион.</span><span class="sxs-lookup"><span data-stu-id="5fb36-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="5fb36-142">Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="5fb36-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="5fb36-143">имажеид</span><span class="sxs-lookup"><span data-stu-id="5fb36-143">imageId</span></span>|<span data-ttu-id="5fb36-144">String</span><span class="sxs-lookup"><span data-stu-id="5fb36-144">String</span></span>|<span data-ttu-id="5fb36-145">Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="5fb36-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="5fb36-146">Формат изображения для типа галереи: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="5fb36-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="5fb36-147">имажедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="5fb36-147">imageDisplayName</span></span>|<span data-ttu-id="5fb36-148">String</span><span class="sxs-lookup"><span data-stu-id="5fb36-148">String</span></span>|<span data-ttu-id="5fb36-149">Отображаемое имя для образа ОС, который вы собираетесь заготовить.</span><span class="sxs-lookup"><span data-stu-id="5fb36-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="5fb36-150">имажетипе</span><span class="sxs-lookup"><span data-stu-id="5fb36-150">imageType</span></span>|<span data-ttu-id="5fb36-151">клаудпкпровисионингполициимажетипе</span><span class="sxs-lookup"><span data-stu-id="5fb36-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="5fb36-152">Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="5fb36-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="5fb36-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="5fb36-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="5fb36-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fb36-154">Response</span></span>

<span data-ttu-id="5fb36-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5fb36-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fb36-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="5fb36-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fb36-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fb36-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5fb36-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fb36-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "gallery"
}
```
# <a name="c"></a>[<span data-ttu-id="5fb36-159">C#</span><span class="sxs-lookup"><span data-stu-id="5fb36-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fb36-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fb36-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fb36-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fb36-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fb36-162">Java</span><span class="sxs-lookup"><span data-stu-id="5fb36-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5fb36-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fb36-163">Response</span></span>

<span data-ttu-id="5fb36-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5fb36-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
  }
```
