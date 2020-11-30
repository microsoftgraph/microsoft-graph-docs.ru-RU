---
title: Создание Клаудпкпровисионингполици
description: Создайте новую политику подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c476ef638a2a1504e04bbb414e1d330416f80a29
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378581"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="85f6e-103">Создание Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="85f6e-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="85f6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85f6e-105">Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="85f6e-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85f6e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85f6e-106">Permissions</span></span>

<span data-ttu-id="85f6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f6e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85f6e-109">Permission type</span></span>|<span data-ttu-id="85f6e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85f6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85f6e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85f6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85f6e-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85f6e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="85f6e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85f6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85f6e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f6e-114">Not supported.</span></span>|
|<span data-ttu-id="85f6e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85f6e-115">Application</span></span>|<span data-ttu-id="85f6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f6e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85f6e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="85f6e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85f6e-118">Request headers</span></span>

| <span data-ttu-id="85f6e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85f6e-119">Name</span></span>          | <span data-ttu-id="85f6e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85f6e-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="85f6e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85f6e-121">Authorization</span></span> | <span data-ttu-id="85f6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85f6e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85f6e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85f6e-124">Content-Type</span></span>  | <span data-ttu-id="85f6e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85f6e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f6e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85f6e-127">Request body</span></span>

<span data-ttu-id="85f6e-128">В тексте запроса добавьте представление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85f6e-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="85f6e-129">В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="85f6e-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="85f6e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85f6e-130">Property</span></span>|<span data-ttu-id="85f6e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85f6e-131">Type</span></span>|<span data-ttu-id="85f6e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85f6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f6e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="85f6e-133">displayName</span></span>|<span data-ttu-id="85f6e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="85f6e-134">String</span></span>|<span data-ttu-id="85f6e-135">Отображаемое имя политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="85f6e-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="85f6e-136">description</span><span class="sxs-lookup"><span data-stu-id="85f6e-136">description</span></span>|<span data-ttu-id="85f6e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="85f6e-137">String</span></span>|<span data-ttu-id="85f6e-138">Описание политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="85f6e-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="85f6e-139">онпремисесконнектионид</span><span class="sxs-lookup"><span data-stu-id="85f6e-139">onPremisesConnectionId</span></span>|<span data-ttu-id="85f6e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="85f6e-140">String</span></span>|<span data-ttu-id="85f6e-141">Идентификатор Клаудпконпремисесконнектион.</span><span class="sxs-lookup"><span data-stu-id="85f6e-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="85f6e-142">Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="85f6e-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="85f6e-143">имажеид</span><span class="sxs-lookup"><span data-stu-id="85f6e-143">imageId</span></span>|<span data-ttu-id="85f6e-144">Строка</span><span class="sxs-lookup"><span data-stu-id="85f6e-144">String</span></span>|<span data-ttu-id="85f6e-145">Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="85f6e-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="85f6e-146">Формат изображения для типа галереи: {publisher_offer_sku}.</span><span class="sxs-lookup"><span data-stu-id="85f6e-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="85f6e-147">имажедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="85f6e-147">imageDisplayName</span></span>|<span data-ttu-id="85f6e-148">Строка</span><span class="sxs-lookup"><span data-stu-id="85f6e-148">String</span></span>|<span data-ttu-id="85f6e-149">Отображаемое имя для образа ОС, который вы собираетесь заготовить.</span><span class="sxs-lookup"><span data-stu-id="85f6e-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="85f6e-150">имажетипе</span><span class="sxs-lookup"><span data-stu-id="85f6e-150">imageType</span></span>|<span data-ttu-id="85f6e-151">клаудпкпровисионингполициимажетипе</span><span class="sxs-lookup"><span data-stu-id="85f6e-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="85f6e-152">Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="85f6e-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="85f6e-153">Возможные значения: `gallery`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="85f6e-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="85f6e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="85f6e-154">Response</span></span>

<span data-ttu-id="85f6e-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85f6e-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85f6e-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="85f6e-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85f6e-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="85f6e-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="85f6e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="85f6e-158">Response</span></span>

<span data-ttu-id="85f6e-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85f6e-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
