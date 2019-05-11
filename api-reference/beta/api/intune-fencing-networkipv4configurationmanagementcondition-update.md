---
title: Обновление networkIPv4ConfigurationManagementCondition
description: Обновление свойств объекта networkIPv4ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19f29064e0fe5bd673c0ffbc0677959b9be844c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905275"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="685ac-103">Обновление networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="685ac-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="685ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="685ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="685ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="685ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="685ac-106">Обновление свойств объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="685ac-106">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="685ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="685ac-107">Prerequisites</span></span>
<span data-ttu-id="685ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="685ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="685ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="685ac-110">Permission type</span></span>|<span data-ttu-id="685ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="685ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="685ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="685ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="685ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="685ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="685ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="685ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="685ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="685ac-115">Not supported.</span></span>|
|<span data-ttu-id="685ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="685ac-116">Application</span></span>|<span data-ttu-id="685ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="685ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="685ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="685ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="685ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="685ac-119">Request headers</span></span>
|<span data-ttu-id="685ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="685ac-120">Header</span></span>|<span data-ttu-id="685ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="685ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="685ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="685ac-122">Authorization</span></span>|<span data-ttu-id="685ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="685ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="685ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="685ac-124">Accept</span></span>|<span data-ttu-id="685ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="685ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="685ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="685ac-126">Request body</span></span>
<span data-ttu-id="685ac-127">В тексте запроса добавьте представление объекта [NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="685ac-127">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="685ac-128">В следующей таблице приведены свойства, необходимые при создании [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="685ac-128">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="685ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="685ac-129">Property</span></span>|<span data-ttu-id="685ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="685ac-130">Type</span></span>|<span data-ttu-id="685ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="685ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="685ac-132">id</span><span class="sxs-lookup"><span data-stu-id="685ac-132">id</span></span>|<span data-ttu-id="685ac-133">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-133">String</span></span>|<span data-ttu-id="685ac-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="685ac-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="685ac-135">System generated value assigned when created.</span></span> <span data-ttu-id="685ac-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="685ac-137">uniqueName</span></span>|<span data-ttu-id="685ac-138">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-138">String</span></span>|<span data-ttu-id="685ac-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-139">Unique name for the management condition.</span></span> <span data-ttu-id="685ac-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-140">Used in management condition expressions.</span></span> <span data-ttu-id="685ac-141">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-142">displayName</span><span class="sxs-lookup"><span data-stu-id="685ac-142">displayName</span></span>|<span data-ttu-id="685ac-143">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-143">String</span></span>|<span data-ttu-id="685ac-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="685ac-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="685ac-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-146">description</span><span class="sxs-lookup"><span data-stu-id="685ac-146">description</span></span>|<span data-ttu-id="685ac-147">String</span><span class="sxs-lookup"><span data-stu-id="685ac-147">String</span></span>|<span data-ttu-id="685ac-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="685ac-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="685ac-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="685ac-150">createdDateTime</span></span>|<span data-ttu-id="685ac-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685ac-151">DateTimeOffset</span></span>|<span data-ttu-id="685ac-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-152">The time the management condition was created.</span></span> <span data-ttu-id="685ac-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="685ac-153">Generated service side.</span></span> <span data-ttu-id="685ac-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="685ac-155">modifiedDateTime</span></span>|<span data-ttu-id="685ac-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685ac-156">DateTimeOffset</span></span>|<span data-ttu-id="685ac-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-157">The time the management condition was last modified.</span></span> <span data-ttu-id="685ac-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="685ac-158">Updated service side.</span></span> <span data-ttu-id="685ac-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-160">eTag</span><span class="sxs-lookup"><span data-stu-id="685ac-160">eTag</span></span>|<span data-ttu-id="685ac-161">String</span><span class="sxs-lookup"><span data-stu-id="685ac-161">String</span></span>|<span data-ttu-id="685ac-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-162">ETag of the management condition.</span></span> <span data-ttu-id="685ac-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="685ac-163">Updated service side.</span></span> <span data-ttu-id="685ac-164">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="685ac-165">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="685ac-165">applicablePlatforms</span></span>|<span data-ttu-id="685ac-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="685ac-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="685ac-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="685ac-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="685ac-168">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="685ac-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="685ac-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="685ac-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="685ac-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="685ac-170">ipV4Prefix</span></span>|<span data-ttu-id="685ac-171">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-171">String</span></span>|<span data-ttu-id="685ac-172">Подсеть IPv4, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="685ac-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="685ac-173">Например, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="685ac-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="685ac-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="685ac-174">ipV4Gateway</span></span>|<span data-ttu-id="685ac-175">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-175">String</span></span>|<span data-ttu-id="685ac-176">IPv4-адрес шлюза.</span><span class="sxs-lookup"><span data-stu-id="685ac-176">The IPv4 gateway address.</span></span> <span data-ttu-id="685ac-177">Например, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="685ac-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="685ac-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="685ac-178">ipV4DHCPServer</span></span>|<span data-ttu-id="685ac-179">Строка</span><span class="sxs-lookup"><span data-stu-id="685ac-179">String</span></span>|<span data-ttu-id="685ac-180">IPv4-адрес DHCP-сервера для адаптера.</span><span class="sxs-lookup"><span data-stu-id="685ac-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="685ac-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="685ac-181">ipV4DNSServerList</span></span>|<span data-ttu-id="685ac-182">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="685ac-182">String collection</span></span>|<span data-ttu-id="685ac-183">DNS-серверы IPv4, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="685ac-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="685ac-184">Днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="685ac-184">dnsSuffixList</span></span>|<span data-ttu-id="685ac-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="685ac-185">String collection</span></span>|<span data-ttu-id="685ac-186">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="685ac-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="685ac-187">Например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="685ac-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="685ac-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="685ac-188">Response</span></span>
<span data-ttu-id="685ac-189">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="685ac-189">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685ac-190">Пример</span><span class="sxs-lookup"><span data-stu-id="685ac-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="685ac-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="685ac-191">Request</span></span>
<span data-ttu-id="685ac-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="685ac-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="685ac-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="685ac-193">Response</span></span>
<span data-ttu-id="685ac-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="685ac-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




