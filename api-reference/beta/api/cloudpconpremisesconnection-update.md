---
title: Обновление Клаудпконпремисесконнектион
description: Обновление свойств объекта Клаудпконпремисесконнектион.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ba7034305d6d8dcabea463e0f98f034947334ac8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563277"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="e8767-103">Обновление Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="e8767-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="e8767-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8767-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8767-105">Обновление свойств объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="e8767-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="e8767-106">После того как локальное подключение проходит проверку работоспособности, которое указывается `healthCheckStatus` свойством, его нельзя обновить.</span><span class="sxs-lookup"><span data-stu-id="e8767-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e8767-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8767-107">Permissions</span></span>

<span data-ttu-id="e8767-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8767-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8767-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8767-110">Permission type</span></span>|<span data-ttu-id="e8767-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8767-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8767-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8767-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8767-113">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8767-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="e8767-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8767-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8767-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8767-115">Not supported.</span></span>|
|<span data-ttu-id="e8767-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8767-116">Application</span></span>|<span data-ttu-id="e8767-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8767-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8767-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8767-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8767-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8767-119">Request headers</span></span>

| <span data-ttu-id="e8767-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e8767-120">Name</span></span>          | <span data-ttu-id="e8767-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e8767-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="e8767-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8767-122">Authorization</span></span> | <span data-ttu-id="e8767-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8767-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8767-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8767-125">Content-Type</span></span>  | <span data-ttu-id="e8767-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8767-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8767-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8767-128">Request body</span></span>

<span data-ttu-id="e8767-129">В тексте запроса добавьте представление объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8767-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="e8767-130">В следующей таблице приведены свойства, необходимые при создании [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="e8767-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="e8767-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8767-131">Property</span></span>|<span data-ttu-id="e8767-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e8767-132">Type</span></span>|<span data-ttu-id="e8767-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e8767-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8767-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e8767-134">displayName</span></span>|<span data-ttu-id="e8767-135">String</span><span class="sxs-lookup"><span data-stu-id="e8767-135">String</span></span>|<span data-ttu-id="e8767-136">Отображаемое имя для локального подключения.</span><span class="sxs-lookup"><span data-stu-id="e8767-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="e8767-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="e8767-137">subscriptionId</span></span>|<span data-ttu-id="e8767-138">String</span><span class="sxs-lookup"><span data-stu-id="e8767-138">String</span></span>|<span data-ttu-id="e8767-139">Идентификатор целевой подписки Azure, связанной с клиентом.</span><span class="sxs-lookup"><span data-stu-id="e8767-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="e8767-140">аддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="e8767-140">adDomainName</span></span>|<span data-ttu-id="e8767-141">String</span><span class="sxs-lookup"><span data-stu-id="e8767-141">String</span></span>|<span data-ttu-id="e8767-142">Полное доменное имя (FQDN) домена Active Directory, к которому нужно присоединиться.</span><span class="sxs-lookup"><span data-stu-id="e8767-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="e8767-143">аддомаинусернаме</span><span class="sxs-lookup"><span data-stu-id="e8767-143">adDomainUsername</span></span>|<span data-ttu-id="e8767-144">String</span><span class="sxs-lookup"><span data-stu-id="e8767-144">String</span></span>|<span data-ttu-id="e8767-145">Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), имеющей разрешения на создание объектов компьютеров в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8767-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="e8767-146">Требуемый формат: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="e8767-146">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="e8767-147">аддомаинпассворд</span><span class="sxs-lookup"><span data-stu-id="e8767-147">adDomainPassword</span></span>|<span data-ttu-id="e8767-148">String</span><span class="sxs-lookup"><span data-stu-id="e8767-148">String</span></span>|<span data-ttu-id="e8767-149">Пароль, связанный с Аддомаинусернаме.</span><span class="sxs-lookup"><span data-stu-id="e8767-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="e8767-150">ресаурцеграупид</span><span class="sxs-lookup"><span data-stu-id="e8767-150">resourceGroupId</span></span>|<span data-ttu-id="e8767-151">String</span><span class="sxs-lookup"><span data-stu-id="e8767-151">String</span></span>|<span data-ttu-id="e8767-152">Идентификатор целевой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e8767-152">The ID of the target resource group.</span></span> <span data-ttu-id="e8767-153">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}".</span><span class="sxs-lookup"><span data-stu-id="e8767-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="e8767-154">виртуалнетворкид</span><span class="sxs-lookup"><span data-stu-id="e8767-154">virtualNetworkId</span></span>|<span data-ttu-id="e8767-155">String</span><span class="sxs-lookup"><span data-stu-id="e8767-155">String</span></span>|<span data-ttu-id="e8767-156">Идентификатор целевой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="e8767-156">The ID of the target virtual network.</span></span> <span data-ttu-id="e8767-157">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкнаме}".</span><span class="sxs-lookup"><span data-stu-id="e8767-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="e8767-158">субнетид</span><span class="sxs-lookup"><span data-stu-id="e8767-158">subnetId</span></span>|<span data-ttu-id="e8767-159">String</span><span class="sxs-lookup"><span data-stu-id="e8767-159">String</span></span>|<span data-ttu-id="e8767-160">Идентификатор целевой подсети.</span><span class="sxs-lookup"><span data-stu-id="e8767-160">The ID of the target subnet.</span></span> <span data-ttu-id="e8767-161">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкид}/субнетс/{субнетнаме}".</span><span class="sxs-lookup"><span data-stu-id="e8767-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="e8767-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8767-162">Response</span></span>

<span data-ttu-id="e8767-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8767-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8767-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8767-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8767-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8767-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e8767-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8767-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e8767-167">C#</span><span class="sxs-lookup"><span data-stu-id="e8767-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8767-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8767-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8767-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8767-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8767-170">Java</span><span class="sxs-lookup"><span data-stu-id="e8767-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8767-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8767-171">Response</span></span>

<span data-ttu-id="e8767-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8767-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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
