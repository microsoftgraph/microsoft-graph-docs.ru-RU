---
title: Обновление cloudPcProvisioningPolicy
description: Обновление свойств объекта cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b070f24cc91562626467aa3b4645e67fffd6d13c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872732"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="835cd-103">Обновление cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="835cd-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="835cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="835cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="835cd-105">Обновление свойств объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="835cd-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="835cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="835cd-106">Permissions</span></span>

<span data-ttu-id="835cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="835cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="835cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="835cd-109">Permission type</span></span>|<span data-ttu-id="835cd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="835cd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="835cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="835cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="835cd-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="835cd-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="835cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="835cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="835cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="835cd-114">Not supported.</span></span>|
|<span data-ttu-id="835cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="835cd-115">Application</span></span>|<span data-ttu-id="835cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="835cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="835cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="835cd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="835cd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="835cd-118">Request headers</span></span>

| <span data-ttu-id="835cd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="835cd-119">Name</span></span>          | <span data-ttu-id="835cd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="835cd-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="835cd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="835cd-121">Authorization</span></span> | <span data-ttu-id="835cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="835cd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="835cd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="835cd-124">Content-Type</span></span>  | <span data-ttu-id="835cd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="835cd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="835cd-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="835cd-127">Request body</span></span>

<span data-ttu-id="835cd-128">В теле запроса укажу представление объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="835cd-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="835cd-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="835cd-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="835cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="835cd-130">Property</span></span>|<span data-ttu-id="835cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="835cd-131">Type</span></span>|<span data-ttu-id="835cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="835cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="835cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="835cd-133">displayName</span></span>|<span data-ttu-id="835cd-134">String</span><span class="sxs-lookup"><span data-stu-id="835cd-134">String</span></span>|<span data-ttu-id="835cd-135">Отображаемого имени для политики предоставления.</span><span class="sxs-lookup"><span data-stu-id="835cd-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="835cd-136">description</span><span class="sxs-lookup"><span data-stu-id="835cd-136">description</span></span>|<span data-ttu-id="835cd-137">String</span><span class="sxs-lookup"><span data-stu-id="835cd-137">String</span></span>|<span data-ttu-id="835cd-138">Описание политики предоставления.</span><span class="sxs-lookup"><span data-stu-id="835cd-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="835cd-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="835cd-139">onPremisesConnectionId</span></span>|<span data-ttu-id="835cd-140">String</span><span class="sxs-lookup"><span data-stu-id="835cd-140">String</span></span>|<span data-ttu-id="835cd-141">ИД cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="835cd-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="835cd-142">Чтобы убедиться, что облачные компьютеры имеют сетевое подключение и присоединяются к домену, выберите подключение к виртуальной сети, проверяемой службой облачных КОМПЬЮТЕРов.</span><span class="sxs-lookup"><span data-stu-id="835cd-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="835cd-143">imageId</span><span class="sxs-lookup"><span data-stu-id="835cd-143">imageId</span></span>|<span data-ttu-id="835cd-144">String</span><span class="sxs-lookup"><span data-stu-id="835cd-144">String</span></span>|<span data-ttu-id="835cd-145">ИД образа ОС, который вы хотите получить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="835cd-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="835cd-146">Формат изображения типа коллекции: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="835cd-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="835cd-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="835cd-147">imageDisplayName</span></span>|<span data-ttu-id="835cd-148">String</span><span class="sxs-lookup"><span data-stu-id="835cd-148">String</span></span>|<span data-ttu-id="835cd-149">Отображаемая имя для образа ОПЕРАЦИОННОй системы, который вы provisioning.</span><span class="sxs-lookup"><span data-stu-id="835cd-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="835cd-150">imageType</span><span class="sxs-lookup"><span data-stu-id="835cd-150">imageType</span></span>|<span data-ttu-id="835cd-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="835cd-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="835cd-152">Тип образа ОС (настраиваемого или галереи), который необходимо настроить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="835cd-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="835cd-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="835cd-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="835cd-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="835cd-154">Response</span></span>

<span data-ttu-id="835cd-155">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="835cd-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="835cd-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="835cd-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="835cd-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="835cd-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="835cd-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="835cd-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="835cd-159">C#</span><span class="sxs-lookup"><span data-stu-id="835cd-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="835cd-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="835cd-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="835cd-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="835cd-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="835cd-162">Java</span><span class="sxs-lookup"><span data-stu-id="835cd-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="835cd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="835cd-163">Response</span></span>

<span data-ttu-id="835cd-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="835cd-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
