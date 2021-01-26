---
title: Обновление cloudPcOnPremisesConnection
description: Обновление свойств объекта cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9c7f71249f47f9027afc8e7495e8d133a9f74885
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981720"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="45a92-103">Обновление cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="45a92-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="45a92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a92-105">Обновление свойств объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="45a92-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="45a92-106">После того как локальное подключение пройдет проверку на состояние, указанную `healthCheckStatus` свойством, вы не сможете обновить его.</span><span class="sxs-lookup"><span data-stu-id="45a92-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="45a92-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45a92-107">Permissions</span></span>

<span data-ttu-id="45a92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a92-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45a92-110">Permission type</span></span>|<span data-ttu-id="45a92-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45a92-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a92-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45a92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45a92-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a92-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="45a92-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45a92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a92-115">Not supported.</span></span>|
|<span data-ttu-id="45a92-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45a92-116">Application</span></span>|<span data-ttu-id="45a92-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a92-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45a92-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45a92-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45a92-119">Request headers</span></span>

| <span data-ttu-id="45a92-120">Имя</span><span class="sxs-lookup"><span data-stu-id="45a92-120">Name</span></span>          | <span data-ttu-id="45a92-121">Описание</span><span class="sxs-lookup"><span data-stu-id="45a92-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="45a92-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45a92-122">Authorization</span></span> | <span data-ttu-id="45a92-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45a92-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="45a92-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45a92-125">Content-Type</span></span>  | <span data-ttu-id="45a92-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45a92-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a92-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45a92-128">Request body</span></span>

<span data-ttu-id="45a92-129">В теле запроса предоставляем представление объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="45a92-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="45a92-130">В следующей таблице показаны свойства, необходимые при создании [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="45a92-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="45a92-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="45a92-131">Property</span></span>|<span data-ttu-id="45a92-132">Тип</span><span class="sxs-lookup"><span data-stu-id="45a92-132">Type</span></span>|<span data-ttu-id="45a92-133">Описание</span><span class="sxs-lookup"><span data-stu-id="45a92-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a92-134">displayName</span><span class="sxs-lookup"><span data-stu-id="45a92-134">displayName</span></span>|<span data-ttu-id="45a92-135">String</span><span class="sxs-lookup"><span data-stu-id="45a92-135">String</span></span>|<span data-ttu-id="45a92-136">Отображаемого имени для локального подключения.</span><span class="sxs-lookup"><span data-stu-id="45a92-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="45a92-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="45a92-137">subscriptionId</span></span>|<span data-ttu-id="45a92-138">String</span><span class="sxs-lookup"><span data-stu-id="45a92-138">String</span></span>|<span data-ttu-id="45a92-139">ИД целевой подписки Azure, связанной с клиентом.</span><span class="sxs-lookup"><span data-stu-id="45a92-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="45a92-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="45a92-140">adDomainName</span></span>|<span data-ttu-id="45a92-141">String</span><span class="sxs-lookup"><span data-stu-id="45a92-141">String</span></span>|<span data-ttu-id="45a92-142">Полное доменное имя домена Active Directory, к нему нужно присоединиться.</span><span class="sxs-lookup"><span data-stu-id="45a92-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="45a92-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="45a92-143">adDomainUsername</span></span>|<span data-ttu-id="45a92-144">String</span><span class="sxs-lookup"><span data-stu-id="45a92-144">String</span></span>|<span data-ttu-id="45a92-145">Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), которая имеет разрешения на создание объектов-компьютеров в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="45a92-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="45a92-146">Необходимый формат: username@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="45a92-146">Required format: username@contoso.com.</span></span>|
|<span data-ttu-id="45a92-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="45a92-147">adDomainPassword</span></span>|<span data-ttu-id="45a92-148">String</span><span class="sxs-lookup"><span data-stu-id="45a92-148">String</span></span>|<span data-ttu-id="45a92-149">Пароль, связанный с adDomainUsername.</span><span class="sxs-lookup"><span data-stu-id="45a92-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="45a92-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="45a92-150">resourceGroupId</span></span>|<span data-ttu-id="45a92-151">String</span><span class="sxs-lookup"><span data-stu-id="45a92-151">String</span></span>|<span data-ttu-id="45a92-152">ИД целевой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="45a92-152">The ID of the target resource group.</span></span> <span data-ttu-id="45a92-153">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span><span class="sxs-lookup"><span data-stu-id="45a92-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="45a92-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="45a92-154">virtualNetworkId</span></span>|<span data-ttu-id="45a92-155">String</span><span class="sxs-lookup"><span data-stu-id="45a92-155">String</span></span>|<span data-ttu-id="45a92-156">ИД целевой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="45a92-156">The ID of the target virtual network.</span></span> <span data-ttu-id="45a92-157">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span><span class="sxs-lookup"><span data-stu-id="45a92-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="45a92-158">subnetId</span><span class="sxs-lookup"><span data-stu-id="45a92-158">subnetId</span></span>|<span data-ttu-id="45a92-159">String</span><span class="sxs-lookup"><span data-stu-id="45a92-159">String</span></span>|<span data-ttu-id="45a92-160">ИД целевой подсети.</span><span class="sxs-lookup"><span data-stu-id="45a92-160">The ID of the target subnet.</span></span> <span data-ttu-id="45a92-161">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span><span class="sxs-lookup"><span data-stu-id="45a92-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="45a92-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="45a92-162">Response</span></span>

<span data-ttu-id="45a92-163">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45a92-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45a92-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="45a92-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45a92-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="45a92-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="45a92-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a92-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisesconnections"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
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
# <a name="c"></a>[<span data-ttu-id="45a92-167">C#</span><span class="sxs-lookup"><span data-stu-id="45a92-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45a92-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45a92-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45a92-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45a92-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45a92-170">Java</span><span class="sxs-lookup"><span data-stu-id="45a92-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45a92-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="45a92-171">Response</span></span>

<span data-ttu-id="45a92-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45a92-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdcc4ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "running",
  "inUse": false
}
```
