---
title: Создание Клаудпконпремисесконнектион
description: Создайте локальное подключение для подготовки облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0cbdbd6cb135e6adecf110ed6d18d03f9dfa5dd9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563468"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="f8741-103">Создание Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="f8741-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="f8741-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8741-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8741-105">Создание нового объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) для подготовки облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="f8741-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f8741-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8741-106">Permissions</span></span>

<span data-ttu-id="f8741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8741-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8741-109">Permission type</span></span>|<span data-ttu-id="f8741-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8741-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8741-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8741-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8741-112">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f8741-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f8741-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8741-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8741-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8741-114">Not supported.</span></span>|
|<span data-ttu-id="f8741-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8741-115">Application</span></span>|<span data-ttu-id="f8741-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8741-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8741-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8741-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="f8741-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8741-118">Request headers</span></span>

| <span data-ttu-id="f8741-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f8741-119">Name</span></span>          | <span data-ttu-id="f8741-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f8741-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="f8741-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8741-121">Authorization</span></span> | <span data-ttu-id="f8741-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8741-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f8741-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8741-124">Content-Type</span></span>  | <span data-ttu-id="f8741-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8741-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8741-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8741-127">Request body</span></span>

<span data-ttu-id="f8741-128">В тексте запроса добавьте представление объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8741-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="f8741-129">В следующей таблице приведены свойства, необходимые при создании [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f8741-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="f8741-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8741-130">Property</span></span>|<span data-ttu-id="f8741-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f8741-131">Type</span></span>|<span data-ttu-id="f8741-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f8741-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8741-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f8741-133">displayName</span></span>|<span data-ttu-id="f8741-134">String</span><span class="sxs-lookup"><span data-stu-id="f8741-134">String</span></span>|<span data-ttu-id="f8741-135">Отображаемое имя для локального подключения.</span><span class="sxs-lookup"><span data-stu-id="f8741-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="f8741-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f8741-136">subscriptionId</span></span>|<span data-ttu-id="f8741-137">String</span><span class="sxs-lookup"><span data-stu-id="f8741-137">String</span></span>|<span data-ttu-id="f8741-138">Идентификатор целевой подписки Azure, связанной с клиентом.</span><span class="sxs-lookup"><span data-stu-id="f8741-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="f8741-139">аддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="f8741-139">adDomainName</span></span>|<span data-ttu-id="f8741-140">String</span><span class="sxs-lookup"><span data-stu-id="f8741-140">String</span></span>|<span data-ttu-id="f8741-141">Полное доменное имя (FQDN) домена Active Directory, к которому нужно присоединиться.</span><span class="sxs-lookup"><span data-stu-id="f8741-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="f8741-142">аддомаинусернаме</span><span class="sxs-lookup"><span data-stu-id="f8741-142">adDomainUsername</span></span>|<span data-ttu-id="f8741-143">String</span><span class="sxs-lookup"><span data-stu-id="f8741-143">String</span></span>|<span data-ttu-id="f8741-144">Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), имеющей разрешения на создание объектов компьютеров в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8741-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="f8741-145">Требуемый формат: contoso@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="f8741-145">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="f8741-146">аддомаинпассворд</span><span class="sxs-lookup"><span data-stu-id="f8741-146">adDomainPassword</span></span>|<span data-ttu-id="f8741-147">String</span><span class="sxs-lookup"><span data-stu-id="f8741-147">String</span></span>|<span data-ttu-id="f8741-148">Пароль, связанный с Аддомаинусернаме.</span><span class="sxs-lookup"><span data-stu-id="f8741-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="f8741-149">ресаурцеграупид</span><span class="sxs-lookup"><span data-stu-id="f8741-149">resourceGroupId</span></span>|<span data-ttu-id="f8741-150">String</span><span class="sxs-lookup"><span data-stu-id="f8741-150">String</span></span>|<span data-ttu-id="f8741-151">Идентификатор целевой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f8741-151">The ID of the target resource group.</span></span> <span data-ttu-id="f8741-152">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}".</span><span class="sxs-lookup"><span data-stu-id="f8741-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="f8741-153">виртуалнетворкид</span><span class="sxs-lookup"><span data-stu-id="f8741-153">virtualNetworkId</span></span>|<span data-ttu-id="f8741-154">String</span><span class="sxs-lookup"><span data-stu-id="f8741-154">String</span></span>|<span data-ttu-id="f8741-155">Идентификатор целевой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="f8741-155">The ID of the target virtual network.</span></span> <span data-ttu-id="f8741-156">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкнаме}".</span><span class="sxs-lookup"><span data-stu-id="f8741-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="f8741-157">субнетид</span><span class="sxs-lookup"><span data-stu-id="f8741-157">subnetId</span></span>|<span data-ttu-id="f8741-158">String</span><span class="sxs-lookup"><span data-stu-id="f8741-158">String</span></span>|<span data-ttu-id="f8741-159">Идентификатор целевой подсети.</span><span class="sxs-lookup"><span data-stu-id="f8741-159">The ID of the target subnet.</span></span> <span data-ttu-id="f8741-160">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкид}/субнетс/{субнетнаме}".</span><span class="sxs-lookup"><span data-stu-id="f8741-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="f8741-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8741-161">Response</span></span>

<span data-ttu-id="f8741-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8741-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8741-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="f8741-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8741-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8741-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8741-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8741-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f8741-166">C#</span><span class="sxs-lookup"><span data-stu-id="f8741-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8741-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8741-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8741-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8741-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8741-169">Java</span><span class="sxs-lookup"><span data-stu-id="f8741-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8741-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8741-170">Response</span></span>

<span data-ttu-id="f8741-171">**Примечание:** Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8741-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="f8741-172">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f8741-172">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8741-173">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8741-173">All of the properties will be returned from an actual call.</span></span>
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
