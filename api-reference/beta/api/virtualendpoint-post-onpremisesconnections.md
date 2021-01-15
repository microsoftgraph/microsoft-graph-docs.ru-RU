---
title: Создание cloudPcOnPremisesConnection
description: Создайте локальное подключение для предоставления облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1b70d772ab6d69640508afa8150779a0b840e29e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873964"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="eff2e-103">Создание cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="eff2e-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="eff2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff2e-105">Создание объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) для предоставления облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="eff2e-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="eff2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eff2e-106">Permissions</span></span>

<span data-ttu-id="eff2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eff2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eff2e-109">Permission type</span></span>|<span data-ttu-id="eff2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eff2e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eff2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eff2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eff2e-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eff2e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="eff2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eff2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eff2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eff2e-114">Not supported.</span></span>|
|<span data-ttu-id="eff2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eff2e-115">Application</span></span>|<span data-ttu-id="eff2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eff2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eff2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eff2e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="eff2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eff2e-118">Request headers</span></span>

| <span data-ttu-id="eff2e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eff2e-119">Name</span></span>          | <span data-ttu-id="eff2e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eff2e-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="eff2e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eff2e-121">Authorization</span></span> | <span data-ttu-id="eff2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eff2e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eff2e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eff2e-124">Content-Type</span></span>  | <span data-ttu-id="eff2e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eff2e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eff2e-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="eff2e-127">Request body</span></span>

<span data-ttu-id="eff2e-128">В теле запроса предоставляем представление объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="eff2e-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="eff2e-129">В следующей таблице показаны свойства, необходимые при создании [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="eff2e-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="eff2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eff2e-130">Property</span></span>|<span data-ttu-id="eff2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eff2e-131">Type</span></span>|<span data-ttu-id="eff2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eff2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eff2e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eff2e-133">displayName</span></span>|<span data-ttu-id="eff2e-134">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-134">String</span></span>|<span data-ttu-id="eff2e-135">Отображаемого имени для локального подключения.</span><span class="sxs-lookup"><span data-stu-id="eff2e-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="eff2e-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="eff2e-136">subscriptionId</span></span>|<span data-ttu-id="eff2e-137">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-137">String</span></span>|<span data-ttu-id="eff2e-138">ИД целевой подписки Azure, связанной с клиентом.</span><span class="sxs-lookup"><span data-stu-id="eff2e-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="eff2e-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="eff2e-139">adDomainName</span></span>|<span data-ttu-id="eff2e-140">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-140">String</span></span>|<span data-ttu-id="eff2e-141">Полное доменное имя домена Active Directory, к нему нужно присоединиться.</span><span class="sxs-lookup"><span data-stu-id="eff2e-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="eff2e-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="eff2e-142">adDomainUsername</span></span>|<span data-ttu-id="eff2e-143">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-143">String</span></span>|<span data-ttu-id="eff2e-144">Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), которая имеет разрешения на создание объектов-компьютеров в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eff2e-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="eff2e-145">Необходимый формат: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="eff2e-145">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="eff2e-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="eff2e-146">adDomainPassword</span></span>|<span data-ttu-id="eff2e-147">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-147">String</span></span>|<span data-ttu-id="eff2e-148">Пароль, связанный с adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="eff2e-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="eff2e-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="eff2e-149">resourceGroupId</span></span>|<span data-ttu-id="eff2e-150">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-150">String</span></span>|<span data-ttu-id="eff2e-151">ИД целевой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="eff2e-151">The ID of the target resource group.</span></span> <span data-ttu-id="eff2e-152">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="eff2e-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="eff2e-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="eff2e-153">virtualNetworkId</span></span>|<span data-ttu-id="eff2e-154">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-154">String</span></span>|<span data-ttu-id="eff2e-155">ИД целевой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="eff2e-155">The ID of the target virtual network.</span></span> <span data-ttu-id="eff2e-156">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="eff2e-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="eff2e-157">subnetId</span><span class="sxs-lookup"><span data-stu-id="eff2e-157">subnetId</span></span>|<span data-ttu-id="eff2e-158">String</span><span class="sxs-lookup"><span data-stu-id="eff2e-158">String</span></span>|<span data-ttu-id="eff2e-159">ИД целевой подсети.</span><span class="sxs-lookup"><span data-stu-id="eff2e-159">The ID of the target subnet.</span></span> <span data-ttu-id="eff2e-160">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="eff2e-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="eff2e-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="eff2e-161">Response</span></span>

<span data-ttu-id="eff2e-162">В случае успеха этот метод возвращает код отклика и объект `201 Created` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eff2e-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eff2e-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="eff2e-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eff2e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="eff2e-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eff2e-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="eff2e-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpconpremisesconnection_from_cloudpconpremisesconnection"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
Content-Type: application/json
Content-length: 800

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
}
```
# <a name="c"></a>[<span data-ttu-id="eff2e-166">C#</span><span class="sxs-lookup"><span data-stu-id="eff2e-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eff2e-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eff2e-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eff2e-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eff2e-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eff2e-169">Java</span><span class="sxs-lookup"><span data-stu-id="eff2e-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eff2e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="eff2e-170">Response</span></span>

<span data-ttu-id="eff2e-171">**Примечание.** Вот пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eff2e-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="eff2e-172">Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="eff2e-172">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eff2e-173">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eff2e-173">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "ac2ad805-167e-49ee-9bef-196c4ce7ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "pending",
  "inUse": false
}
```
