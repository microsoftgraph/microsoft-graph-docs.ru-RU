---
title: Создание networkIPv4ConfigurationManagementCondition
description: Создание нового объекта networkIPv4ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6459876d0ee318ed3d855a5ff03cb43599773ca3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532151"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="e2571-103">Создание networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="e2571-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="e2571-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2571-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2571-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2571-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2571-106">Создание нового объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="e2571-106">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2571-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2571-107">Prerequisites</span></span>
<span data-ttu-id="e2571-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2571-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2571-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2571-110">Permission type</span></span>|<span data-ttu-id="e2571-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2571-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2571-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2571-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2571-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2571-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2571-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2571-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2571-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2571-115">Not supported.</span></span>|
|<span data-ttu-id="e2571-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2571-116">Application</span></span>|<span data-ttu-id="e2571-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2571-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2571-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2571-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="e2571-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2571-119">Request headers</span></span>
|<span data-ttu-id="e2571-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2571-120">Header</span></span>|<span data-ttu-id="e2571-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e2571-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2571-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2571-122">Authorization</span></span>|<span data-ttu-id="e2571-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2571-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2571-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2571-124">Accept</span></span>|<span data-ttu-id="e2571-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2571-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2571-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2571-126">Request body</span></span>
<span data-ttu-id="e2571-127">В тексте запроса добавьте представление объекта networkIPv4ConfigurationManagementCondition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2571-127">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="e2571-128">В следующей таблице приведены свойства, необходимые при создании networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="e2571-128">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="e2571-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2571-129">Property</span></span>|<span data-ttu-id="e2571-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e2571-130">Type</span></span>|<span data-ttu-id="e2571-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e2571-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2571-132">id</span><span class="sxs-lookup"><span data-stu-id="e2571-132">id</span></span>|<span data-ttu-id="e2571-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e2571-133">String</span></span>|<span data-ttu-id="e2571-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="e2571-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="e2571-135">System generated value assigned when created.</span></span> <span data-ttu-id="e2571-136">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="e2571-137">uniqueName</span></span>|<span data-ttu-id="e2571-138">String</span><span class="sxs-lookup"><span data-stu-id="e2571-138">String</span></span>|<span data-ttu-id="e2571-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-139">Unique name for the management condition.</span></span> <span data-ttu-id="e2571-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-140">Used in management condition expressions.</span></span> <span data-ttu-id="e2571-141">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e2571-142">displayName</span></span>|<span data-ttu-id="e2571-143">String</span><span class="sxs-lookup"><span data-stu-id="e2571-143">String</span></span>|<span data-ttu-id="e2571-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="e2571-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="e2571-145">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-146">description</span><span class="sxs-lookup"><span data-stu-id="e2571-146">description</span></span>|<span data-ttu-id="e2571-147">String</span><span class="sxs-lookup"><span data-stu-id="e2571-147">String</span></span>|<span data-ttu-id="e2571-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="e2571-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="e2571-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2571-150">createdDateTime</span></span>|<span data-ttu-id="e2571-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2571-151">DateTimeOffset</span></span>|<span data-ttu-id="e2571-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-152">The time the management condition was created.</span></span> <span data-ttu-id="e2571-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e2571-153">Generated service side.</span></span> <span data-ttu-id="e2571-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2571-155">modifiedDateTime</span></span>|<span data-ttu-id="e2571-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2571-156">DateTimeOffset</span></span>|<span data-ttu-id="e2571-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-157">The time the management condition was last modified.</span></span> <span data-ttu-id="e2571-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e2571-158">Updated service side.</span></span> <span data-ttu-id="e2571-159">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-160">eTag</span><span class="sxs-lookup"><span data-stu-id="e2571-160">eTag</span></span>|<span data-ttu-id="e2571-161">String</span><span class="sxs-lookup"><span data-stu-id="e2571-161">String</span></span>|<span data-ttu-id="e2571-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-162">ETag of the management condition.</span></span> <span data-ttu-id="e2571-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e2571-163">Updated service side.</span></span> <span data-ttu-id="e2571-164">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e2571-165">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="e2571-165">applicablePlatforms</span></span>|<span data-ttu-id="e2571-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="e2571-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e2571-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="e2571-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="e2571-168">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="e2571-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="e2571-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="e2571-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="e2571-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="e2571-170">ipV4Prefix</span></span>|<span data-ttu-id="e2571-171">String</span><span class="sxs-lookup"><span data-stu-id="e2571-171">String</span></span>|<span data-ttu-id="e2571-172">Подсеть IPv4, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="e2571-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="e2571-173">Например, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="e2571-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="e2571-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="e2571-174">ipV4Gateway</span></span>|<span data-ttu-id="e2571-175">String</span><span class="sxs-lookup"><span data-stu-id="e2571-175">String</span></span>|<span data-ttu-id="e2571-176">IPv4-адрес шлюза.</span><span class="sxs-lookup"><span data-stu-id="e2571-176">The IPv4 gateway address.</span></span> <span data-ttu-id="e2571-177">Например, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="e2571-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="e2571-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="e2571-178">ipV4DHCPServer</span></span>|<span data-ttu-id="e2571-179">String</span><span class="sxs-lookup"><span data-stu-id="e2571-179">String</span></span>|<span data-ttu-id="e2571-180">IPv4-адрес DHCP-сервера для адаптера.</span><span class="sxs-lookup"><span data-stu-id="e2571-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="e2571-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="e2571-181">ipV4DNSServerList</span></span>|<span data-ttu-id="e2571-182">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e2571-182">String collection</span></span>|<span data-ttu-id="e2571-183">DNS-серверы IPv4, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="e2571-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="e2571-184">Днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="e2571-184">dnsSuffixList</span></span>|<span data-ttu-id="e2571-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e2571-185">String collection</span></span>|<span data-ttu-id="e2571-186">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="e2571-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="e2571-187">Например, Seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="e2571-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="e2571-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2571-188">Response</span></span>
<span data-ttu-id="e2571-189">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2571-189">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2571-190">Пример</span><span class="sxs-lookup"><span data-stu-id="e2571-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2571-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2571-191">Request</span></span>
<span data-ttu-id="e2571-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2571-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2571-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2571-193">Response</span></span>
<span data-ttu-id="e2571-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2571-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





