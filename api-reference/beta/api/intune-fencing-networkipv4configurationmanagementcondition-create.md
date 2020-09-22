---
title: Создание networkIPv4ConfigurationManagementCondition
description: Создание нового объекта networkIPv4ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f93f955628f2379ce191cbb8fd584d52866eaf3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054079"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="f1179-103">Создание networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f1179-103">Create networkIPv4ConfigurationManagementCondition</span></span>

<span data-ttu-id="f1179-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1179-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1179-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1179-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1179-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1179-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1179-107">Создание нового объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f1179-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1179-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1179-108">Prerequisites</span></span>
<span data-ttu-id="f1179-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1179-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1179-111">Permission type</span></span>|<span data-ttu-id="f1179-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1179-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1179-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1179-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1179-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1179-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1179-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1179-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1179-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1179-116">Not supported.</span></span>|
|<span data-ttu-id="f1179-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1179-117">Application</span></span>|<span data-ttu-id="f1179-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1179-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1179-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1179-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="f1179-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1179-120">Request headers</span></span>
|<span data-ttu-id="f1179-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1179-121">Header</span></span>|<span data-ttu-id="f1179-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1179-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1179-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1179-123">Authorization</span></span>|<span data-ttu-id="f1179-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1179-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1179-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1179-125">Accept</span></span>|<span data-ttu-id="f1179-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1179-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1179-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1179-127">Request body</span></span>
<span data-ttu-id="f1179-128">В тексте запроса добавьте представление объекта networkIPv4ConfigurationManagementCondition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1179-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="f1179-129">В следующей таблице приведены свойства, необходимые при создании networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="f1179-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="f1179-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1179-130">Property</span></span>|<span data-ttu-id="f1179-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1179-131">Type</span></span>|<span data-ttu-id="f1179-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1179-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1179-133">id</span><span class="sxs-lookup"><span data-stu-id="f1179-133">id</span></span>|<span data-ttu-id="f1179-134">String</span><span class="sxs-lookup"><span data-stu-id="f1179-134">String</span></span>|<span data-ttu-id="f1179-135">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="f1179-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="f1179-136">System generated value assigned when created.</span></span> <span data-ttu-id="f1179-137">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f1179-138">uniqueName</span></span>|<span data-ttu-id="f1179-139">String</span><span class="sxs-lookup"><span data-stu-id="f1179-139">String</span></span>|<span data-ttu-id="f1179-140">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-140">Unique name for the management condition.</span></span> <span data-ttu-id="f1179-141">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-141">Used in management condition expressions.</span></span> <span data-ttu-id="f1179-142">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f1179-143">displayName</span></span>|<span data-ttu-id="f1179-144">String</span><span class="sxs-lookup"><span data-stu-id="f1179-144">String</span></span>|<span data-ttu-id="f1179-145">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="f1179-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="f1179-146">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-147">description</span><span class="sxs-lookup"><span data-stu-id="f1179-147">description</span></span>|<span data-ttu-id="f1179-148">String</span><span class="sxs-lookup"><span data-stu-id="f1179-148">String</span></span>|<span data-ttu-id="f1179-149">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="f1179-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="f1179-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1179-151">createdDateTime</span></span>|<span data-ttu-id="f1179-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1179-152">DateTimeOffset</span></span>|<span data-ttu-id="f1179-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-153">The time the management condition was created.</span></span> <span data-ttu-id="f1179-154">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1179-154">Generated service side.</span></span> <span data-ttu-id="f1179-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1179-156">modifiedDateTime</span></span>|<span data-ttu-id="f1179-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1179-157">DateTimeOffset</span></span>|<span data-ttu-id="f1179-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-158">The time the management condition was last modified.</span></span> <span data-ttu-id="f1179-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1179-159">Updated service side.</span></span> <span data-ttu-id="f1179-160">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-161">eTag</span><span class="sxs-lookup"><span data-stu-id="f1179-161">eTag</span></span>|<span data-ttu-id="f1179-162">String</span><span class="sxs-lookup"><span data-stu-id="f1179-162">String</span></span>|<span data-ttu-id="f1179-163">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-163">ETag of the management condition.</span></span> <span data-ttu-id="f1179-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1179-164">Updated service side.</span></span> <span data-ttu-id="f1179-165">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1179-166">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="f1179-166">applicablePlatforms</span></span>|<span data-ttu-id="f1179-167">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f1179-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f1179-168">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1179-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f1179-169">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f1179-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f1179-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f1179-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="f1179-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="f1179-171">ipV4Prefix</span></span>|<span data-ttu-id="f1179-172">String</span><span class="sxs-lookup"><span data-stu-id="f1179-172">String</span></span>|<span data-ttu-id="f1179-173">Подсеть IPv4, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="f1179-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="f1179-174">Например, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="f1179-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="f1179-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="f1179-175">ipV4Gateway</span></span>|<span data-ttu-id="f1179-176">String</span><span class="sxs-lookup"><span data-stu-id="f1179-176">String</span></span>|<span data-ttu-id="f1179-177">IPv4-адрес шлюза.</span><span class="sxs-lookup"><span data-stu-id="f1179-177">The IPv4 gateway address.</span></span> <span data-ttu-id="f1179-178">Например, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="f1179-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="f1179-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="f1179-179">ipV4DHCPServer</span></span>|<span data-ttu-id="f1179-180">String</span><span class="sxs-lookup"><span data-stu-id="f1179-180">String</span></span>|<span data-ttu-id="f1179-181">IPv4-адрес DHCP-сервера для адаптера.</span><span class="sxs-lookup"><span data-stu-id="f1179-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="f1179-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="f1179-182">ipV4DNSServerList</span></span>|<span data-ttu-id="f1179-183">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f1179-183">String collection</span></span>|<span data-ttu-id="f1179-184">DNS-серверы IPv4, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="f1179-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="f1179-185">днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="f1179-185">dnsSuffixList</span></span>|<span data-ttu-id="f1179-186">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f1179-186">String collection</span></span>|<span data-ttu-id="f1179-187">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="f1179-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="f1179-188">Например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="f1179-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="f1179-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1179-189">Response</span></span>
<span data-ttu-id="f1179-190">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1179-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1179-191">Пример</span><span class="sxs-lookup"><span data-stu-id="f1179-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1179-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1179-192">Request</span></span>
<span data-ttu-id="f1179-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1179-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f1179-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1179-194">Response</span></span>
<span data-ttu-id="f1179-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1179-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```






