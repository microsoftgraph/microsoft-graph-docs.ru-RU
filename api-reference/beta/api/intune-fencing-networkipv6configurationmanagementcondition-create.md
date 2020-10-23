---
title: Создание networkIPv6ConfigurationManagementCondition
description: Создание нового объекта networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a648b15e0ae829bfe5687ef22bb64cb0f48e238e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701916"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="08fe4-103">Создание networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="08fe4-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="08fe4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08fe4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08fe4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fe4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08fe4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08fe4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08fe4-107">Создание нового объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="08fe4-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08fe4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08fe4-108">Prerequisites</span></span>
<span data-ttu-id="08fe4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08fe4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08fe4-111">Permission type</span></span>|<span data-ttu-id="08fe4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08fe4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08fe4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08fe4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08fe4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fe4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08fe4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08fe4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08fe4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fe4-116">Not supported.</span></span>|
|<span data-ttu-id="08fe4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08fe4-117">Application</span></span>|<span data-ttu-id="08fe4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fe4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08fe4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08fe4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="08fe4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08fe4-120">Request headers</span></span>
|<span data-ttu-id="08fe4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08fe4-121">Header</span></span>|<span data-ttu-id="08fe4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08fe4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08fe4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08fe4-123">Authorization</span></span>|<span data-ttu-id="08fe4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08fe4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08fe4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08fe4-125">Accept</span></span>|<span data-ttu-id="08fe4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08fe4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fe4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08fe4-127">Request body</span></span>
<span data-ttu-id="08fe4-128">В тексте запроса добавьте представление объекта networkIPv6ConfigurationManagementCondition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08fe4-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="08fe4-129">В следующей таблице приведены свойства, необходимые при создании networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="08fe4-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="08fe4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08fe4-130">Property</span></span>|<span data-ttu-id="08fe4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08fe4-131">Type</span></span>|<span data-ttu-id="08fe4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08fe4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fe4-133">id</span><span class="sxs-lookup"><span data-stu-id="08fe4-133">id</span></span>|<span data-ttu-id="08fe4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-134">String</span></span>|<span data-ttu-id="08fe4-135">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="08fe4-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="08fe4-136">System generated value assigned when created.</span></span> <span data-ttu-id="08fe4-137">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="08fe4-138">uniqueName</span></span>|<span data-ttu-id="08fe4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-139">String</span></span>|<span data-ttu-id="08fe4-140">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-140">Unique name for the management condition.</span></span> <span data-ttu-id="08fe4-141">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-141">Used in management condition expressions.</span></span> <span data-ttu-id="08fe4-142">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="08fe4-143">displayName</span></span>|<span data-ttu-id="08fe4-144">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-144">String</span></span>|<span data-ttu-id="08fe4-145">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="08fe4-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="08fe4-146">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-147">description</span><span class="sxs-lookup"><span data-stu-id="08fe4-147">description</span></span>|<span data-ttu-id="08fe4-148">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-148">String</span></span>|<span data-ttu-id="08fe4-149">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="08fe4-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="08fe4-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08fe4-151">createdDateTime</span></span>|<span data-ttu-id="08fe4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fe4-152">DateTimeOffset</span></span>|<span data-ttu-id="08fe4-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-153">The time the management condition was created.</span></span> <span data-ttu-id="08fe4-154">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="08fe4-154">Generated service side.</span></span> <span data-ttu-id="08fe4-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08fe4-156">modifiedDateTime</span></span>|<span data-ttu-id="08fe4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fe4-157">DateTimeOffset</span></span>|<span data-ttu-id="08fe4-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-158">The time the management condition was last modified.</span></span> <span data-ttu-id="08fe4-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="08fe4-159">Updated service side.</span></span> <span data-ttu-id="08fe4-160">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-161">eTag</span><span class="sxs-lookup"><span data-stu-id="08fe4-161">eTag</span></span>|<span data-ttu-id="08fe4-162">String</span><span class="sxs-lookup"><span data-stu-id="08fe4-162">String</span></span>|<span data-ttu-id="08fe4-163">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-163">ETag of the management condition.</span></span> <span data-ttu-id="08fe4-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="08fe4-164">Updated service side.</span></span> <span data-ttu-id="08fe4-165">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="08fe4-166">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="08fe4-166">applicablePlatforms</span></span>|<span data-ttu-id="08fe4-167">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="08fe4-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="08fe4-168">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="08fe4-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="08fe4-169">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="08fe4-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="08fe4-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="08fe4-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="08fe4-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="08fe4-171">ipV6Prefix</span></span>|<span data-ttu-id="08fe4-172">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-172">String</span></span>|<span data-ttu-id="08fe4-173">Подсеть IPv6, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="08fe4-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="08fe4-174">Например: 2001: db8::/32</span><span class="sxs-lookup"><span data-stu-id="08fe4-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="08fe4-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="08fe4-175">ipV6Gateway</span></span>|<span data-ttu-id="08fe4-176">Строка</span><span class="sxs-lookup"><span data-stu-id="08fe4-176">String</span></span>|<span data-ttu-id="08fe4-177">Адрес шлюза IPv6 в.</span><span class="sxs-lookup"><span data-stu-id="08fe4-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="08fe4-178">Например, 2001: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="08fe4-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="08fe4-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="08fe4-179">ipV6DNSServerList</span></span>|<span data-ttu-id="08fe4-180">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08fe4-180">String collection</span></span>|<span data-ttu-id="08fe4-181">DNS-серверы IPv6, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="08fe4-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="08fe4-182">днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="08fe4-182">dnsSuffixList</span></span>|<span data-ttu-id="08fe4-183">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08fe4-183">String collection</span></span>|<span data-ttu-id="08fe4-184">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="08fe4-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="08fe4-185">Например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="08fe4-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="08fe4-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="08fe4-186">Response</span></span>
<span data-ttu-id="08fe4-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08fe4-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fe4-188">Пример</span><span class="sxs-lookup"><span data-stu-id="08fe4-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="08fe4-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="08fe4-189">Request</span></span>
<span data-ttu-id="08fe4-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08fe4-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="08fe4-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fe4-191">Response</span></span>
<span data-ttu-id="08fe4-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08fe4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





