---
title: Создание networkIPv6ConfigurationManagementCondition
description: Создайте новый объект networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd802fa20e6abdd04c819a03a259acb47ead0883
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142102"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="77a1f-103">Создание networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="77a1f-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="77a1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77a1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77a1f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77a1f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77a1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77a1f-107">Создайте новый [объект networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77a1f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77a1f-108">Prerequisites</span></span>
<span data-ttu-id="77a1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77a1f-111">Permission type</span></span>|<span data-ttu-id="77a1f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77a1f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77a1f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77a1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77a1f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a1f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77a1f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77a1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77a1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a1f-116">Not supported.</span></span>|
|<span data-ttu-id="77a1f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77a1f-117">Application</span></span>|<span data-ttu-id="77a1f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a1f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77a1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77a1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="77a1f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77a1f-120">Request headers</span></span>
|<span data-ttu-id="77a1f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77a1f-121">Header</span></span>|<span data-ttu-id="77a1f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77a1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77a1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a1f-123">Authorization</span></span>|<span data-ttu-id="77a1f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77a1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77a1f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77a1f-125">Accept</span></span>|<span data-ttu-id="77a1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77a1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77a1f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77a1f-127">Request body</span></span>
<span data-ttu-id="77a1f-128">В теле запроса поставляем представление JSON для объекта networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="77a1f-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="77a1f-129">В следующей таблице показаны свойства, необходимые при создании networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="77a1f-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="77a1f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77a1f-130">Property</span></span>|<span data-ttu-id="77a1f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77a1f-131">Type</span></span>|<span data-ttu-id="77a1f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77a1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77a1f-133">id</span><span class="sxs-lookup"><span data-stu-id="77a1f-133">id</span></span>|<span data-ttu-id="77a1f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-134">String</span></span>|<span data-ttu-id="77a1f-135">Уникальный идентификатор для состояния управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="77a1f-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="77a1f-136">System generated value assigned when created.</span></span> <span data-ttu-id="77a1f-137">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="77a1f-138">uniqueName</span></span>|<span data-ttu-id="77a1f-139">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-139">String</span></span>|<span data-ttu-id="77a1f-140">Уникальное имя для состояния управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-140">Unique name for the management condition.</span></span> <span data-ttu-id="77a1f-141">Используется в выражениях условий управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-141">Used in management condition expressions.</span></span> <span data-ttu-id="77a1f-142">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="77a1f-143">displayName</span></span>|<span data-ttu-id="77a1f-144">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-144">String</span></span>|<span data-ttu-id="77a1f-145">Администратор определил имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="77a1f-146">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-147">description</span><span class="sxs-lookup"><span data-stu-id="77a1f-147">description</span></span>|<span data-ttu-id="77a1f-148">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-148">String</span></span>|<span data-ttu-id="77a1f-149">Администратор определил описание условия управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="77a1f-150">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77a1f-151">createdDateTime</span></span>|<span data-ttu-id="77a1f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a1f-152">DateTimeOffset</span></span>|<span data-ttu-id="77a1f-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-153">The time the management condition was created.</span></span> <span data-ttu-id="77a1f-154">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="77a1f-154">Generated service side.</span></span> <span data-ttu-id="77a1f-155">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77a1f-156">modifiedDateTime</span></span>|<span data-ttu-id="77a1f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a1f-157">DateTimeOffset</span></span>|<span data-ttu-id="77a1f-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-158">The time the management condition was last modified.</span></span> <span data-ttu-id="77a1f-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="77a1f-159">Updated service side.</span></span> <span data-ttu-id="77a1f-160">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-161">eTag</span><span class="sxs-lookup"><span data-stu-id="77a1f-161">eTag</span></span>|<span data-ttu-id="77a1f-162">String</span><span class="sxs-lookup"><span data-stu-id="77a1f-162">String</span></span>|<span data-ttu-id="77a1f-163">ETag состояния управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-163">ETag of the management condition.</span></span> <span data-ttu-id="77a1f-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="77a1f-164">Updated service side.</span></span> <span data-ttu-id="77a1f-165">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="77a1f-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="77a1f-166">applicablePlatforms</span></span>|<span data-ttu-id="77a1f-167">[коллекция devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="77a1f-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="77a1f-168">Применимые платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="77a1f-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="77a1f-169">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="77a1f-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="77a1f-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="77a1f-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="77a1f-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="77a1f-171">ipV6Prefix</span></span>|<span data-ttu-id="77a1f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-172">String</span></span>|<span data-ttu-id="77a1f-173">Подсеть IPv6, к которая должна быть подключена.</span><span class="sxs-lookup"><span data-stu-id="77a1f-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="77a1f-174">например, 2001:db8::/32</span><span class="sxs-lookup"><span data-stu-id="77a1f-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="77a1f-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="77a1f-175">ipV6Gateway</span></span>|<span data-ttu-id="77a1f-176">Строка</span><span class="sxs-lookup"><span data-stu-id="77a1f-176">String</span></span>|<span data-ttu-id="77a1f-177">Адрес шлюза IPv6.</span><span class="sxs-lookup"><span data-stu-id="77a1f-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="77a1f-178">например, 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="77a1f-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="77a1f-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="77a1f-179">ipV6DNSServerList</span></span>|<span data-ttu-id="77a1f-180">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77a1f-180">String collection</span></span>|<span data-ttu-id="77a1f-181">DNS-серверы IPv6, настроенные для адаптеров.</span><span class="sxs-lookup"><span data-stu-id="77a1f-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="77a1f-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="77a1f-182">dnsSuffixList</span></span>|<span data-ttu-id="77a1f-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77a1f-183">String collection</span></span>|<span data-ttu-id="77a1f-184">Допустимые Суффиксы DNS для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="77a1f-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="77a1f-185">например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="77a1f-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="77a1f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="77a1f-186">Response</span></span>
<span data-ttu-id="77a1f-187">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="77a1f-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77a1f-188">Пример</span><span class="sxs-lookup"><span data-stu-id="77a1f-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="77a1f-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="77a1f-189">Request</span></span>
<span data-ttu-id="77a1f-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77a1f-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77a1f-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="77a1f-191">Response</span></span>
<span data-ttu-id="77a1f-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77a1f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




