---
title: Создание cloudPcProvisioningPolicy
description: Создайте новую политику продюсинга облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6c28d27cced97d2e1ab927de14d888ae15d8e902
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547613"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="65e7a-103">Создание cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="65e7a-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="65e7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65e7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65e7a-105">Создайте новый [объект cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65e7a-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="65e7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65e7a-106">Permissions</span></span>

<span data-ttu-id="65e7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65e7a-109">Permission type</span></span>|<span data-ttu-id="65e7a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65e7a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65e7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65e7a-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e7a-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="65e7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65e7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e7a-114">Not supported.</span></span>|
|<span data-ttu-id="65e7a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="65e7a-115">Application</span></span>|<span data-ttu-id="65e7a-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e7a-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65e7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="65e7a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65e7a-118">Request headers</span></span>

| <span data-ttu-id="65e7a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="65e7a-119">Name</span></span>          | <span data-ttu-id="65e7a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65e7a-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="65e7a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65e7a-121">Authorization</span></span> | <span data-ttu-id="65e7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65e7a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65e7a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65e7a-124">Content-Type</span></span>  | <span data-ttu-id="65e7a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65e7a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65e7a-127">Request body</span></span>

<span data-ttu-id="65e7a-128">В теле запроса поставляем представление JSON объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65e7a-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="65e7a-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65e7a-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="65e7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65e7a-130">Property</span></span>|<span data-ttu-id="65e7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65e7a-131">Type</span></span>|<span data-ttu-id="65e7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65e7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e7a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="65e7a-133">displayName</span></span>|<span data-ttu-id="65e7a-134">String</span><span class="sxs-lookup"><span data-stu-id="65e7a-134">String</span></span>|<span data-ttu-id="65e7a-135">Имя отображения политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="65e7a-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="65e7a-136">description</span><span class="sxs-lookup"><span data-stu-id="65e7a-136">description</span></span>|<span data-ttu-id="65e7a-137">String</span><span class="sxs-lookup"><span data-stu-id="65e7a-137">String</span></span>|<span data-ttu-id="65e7a-138">Описание политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="65e7a-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="65e7a-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="65e7a-139">onPremisesConnectionId</span></span>|<span data-ttu-id="65e7a-140">String</span><span class="sxs-lookup"><span data-stu-id="65e7a-140">String</span></span>|<span data-ttu-id="65e7a-141">ID cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="65e7a-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="65e7a-142">Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенное службой облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="65e7a-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="65e7a-143">imageId</span><span class="sxs-lookup"><span data-stu-id="65e7a-143">imageId</span></span>|<span data-ttu-id="65e7a-144">String</span><span class="sxs-lookup"><span data-stu-id="65e7a-144">String</span></span>|<span data-ttu-id="65e7a-145">ID изображения ОС, которое необходимо уладить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="65e7a-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="65e7a-146">Формат изображения типа галереи: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="65e7a-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="65e7a-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="65e7a-147">imageDisplayName</span></span>|<span data-ttu-id="65e7a-148">String</span><span class="sxs-lookup"><span data-stu-id="65e7a-148">String</span></span>|<span data-ttu-id="65e7a-149">Имя отображения образа ОС, которое вы закаповыватель.</span><span class="sxs-lookup"><span data-stu-id="65e7a-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="65e7a-150">imageType</span><span class="sxs-lookup"><span data-stu-id="65e7a-150">imageType</span></span>|<span data-ttu-id="65e7a-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="65e7a-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="65e7a-152">Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="65e7a-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="65e7a-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="65e7a-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="65e7a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="65e7a-154">Response</span></span>

<span data-ttu-id="65e7a-155">В случае успеха этот метод возвращает код отклика и `201 Created` [объект cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="65e7a-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65e7a-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="65e7a-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65e7a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="65e7a-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="65e7a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="65e7a-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="65e7a-159">C#</span><span class="sxs-lookup"><span data-stu-id="65e7a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65e7a-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65e7a-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65e7a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65e7a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65e7a-162">Java</span><span class="sxs-lookup"><span data-stu-id="65e7a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65e7a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="65e7a-163">Response</span></span>

<span data-ttu-id="65e7a-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65e7a-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
