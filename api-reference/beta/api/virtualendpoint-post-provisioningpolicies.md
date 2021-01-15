---
title: Создание cloudPcProvisioningPolicy
description: Создайте новую политику предоставления облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a83b156808fd0c9634fc8c7fedf62a6c9b8a2996
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874076"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="37571-103">Создание cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="37571-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="37571-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37571-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37571-105">Создание объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37571-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="37571-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37571-106">Permissions</span></span>

<span data-ttu-id="37571-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37571-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37571-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37571-109">Permission type</span></span>|<span data-ttu-id="37571-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37571-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37571-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37571-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37571-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37571-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="37571-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37571-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37571-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37571-114">Not supported.</span></span>|
|<span data-ttu-id="37571-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37571-115">Application</span></span>|<span data-ttu-id="37571-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37571-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37571-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37571-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="37571-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37571-118">Request headers</span></span>

| <span data-ttu-id="37571-119">Имя</span><span class="sxs-lookup"><span data-stu-id="37571-119">Name</span></span>          | <span data-ttu-id="37571-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37571-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="37571-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37571-121">Authorization</span></span> | <span data-ttu-id="37571-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37571-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37571-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37571-124">Content-Type</span></span>  | <span data-ttu-id="37571-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37571-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37571-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="37571-127">Request body</span></span>

<span data-ttu-id="37571-128">В теле запроса укажу представление объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="37571-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="37571-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37571-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="37571-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="37571-130">Property</span></span>|<span data-ttu-id="37571-131">Тип</span><span class="sxs-lookup"><span data-stu-id="37571-131">Type</span></span>|<span data-ttu-id="37571-132">Описание</span><span class="sxs-lookup"><span data-stu-id="37571-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37571-133">displayName</span><span class="sxs-lookup"><span data-stu-id="37571-133">displayName</span></span>|<span data-ttu-id="37571-134">String</span><span class="sxs-lookup"><span data-stu-id="37571-134">String</span></span>|<span data-ttu-id="37571-135">Отображаемого имени для политики предоставления.</span><span class="sxs-lookup"><span data-stu-id="37571-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="37571-136">description</span><span class="sxs-lookup"><span data-stu-id="37571-136">description</span></span>|<span data-ttu-id="37571-137">String</span><span class="sxs-lookup"><span data-stu-id="37571-137">String</span></span>|<span data-ttu-id="37571-138">Описание политики предоставления.</span><span class="sxs-lookup"><span data-stu-id="37571-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="37571-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="37571-139">onPremisesConnectionId</span></span>|<span data-ttu-id="37571-140">String</span><span class="sxs-lookup"><span data-stu-id="37571-140">String</span></span>|<span data-ttu-id="37571-141">ИД cloudPcOnPremisesConnection.</span><span class="sxs-lookup"><span data-stu-id="37571-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="37571-142">Чтобы убедиться, что облачные компьютеры имеют сетевое подключение и присоединяются к домену, выберите подключение к виртуальной сети, проверяемой службой облачных КОМПЬЮТЕРов.</span><span class="sxs-lookup"><span data-stu-id="37571-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="37571-143">imageId</span><span class="sxs-lookup"><span data-stu-id="37571-143">imageId</span></span>|<span data-ttu-id="37571-144">String</span><span class="sxs-lookup"><span data-stu-id="37571-144">String</span></span>|<span data-ttu-id="37571-145">ИД образа ОС, который вы хотите получить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="37571-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="37571-146">Формат изображения типа коллекции: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="37571-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="37571-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="37571-147">imageDisplayName</span></span>|<span data-ttu-id="37571-148">String</span><span class="sxs-lookup"><span data-stu-id="37571-148">String</span></span>|<span data-ttu-id="37571-149">Отображаемая имя для образа ОПЕРАЦИОННОй системы, который вы хотите демонстрировать.</span><span class="sxs-lookup"><span data-stu-id="37571-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="37571-150">imageType</span><span class="sxs-lookup"><span data-stu-id="37571-150">imageType</span></span>|<span data-ttu-id="37571-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="37571-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="37571-152">Тип образа ОС (настраиваемого или галереи), который необходимо настроить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="37571-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="37571-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="37571-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="37571-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="37571-154">Response</span></span>

<span data-ttu-id="37571-155">В случае успеха этот метод возвращает код отклика и объект `201 Created` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37571-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37571-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="37571-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37571-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="37571-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37571-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="37571-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37571-159">C#</span><span class="sxs-lookup"><span data-stu-id="37571-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37571-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37571-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37571-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37571-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37571-162">Java</span><span class="sxs-lookup"><span data-stu-id="37571-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37571-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="37571-163">Response</span></span>

<span data-ttu-id="37571-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37571-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
