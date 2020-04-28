---
title: Создание networkIPv6ConfigurationManagementCondition
description: Создание нового объекта networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c97e39babe6ee9330ad86314a9347b743f1571c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384331"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="cef07-103">Создание networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cef07-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="cef07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cef07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cef07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cef07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cef07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cef07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cef07-107">Создание нового объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cef07-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cef07-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cef07-108">Prerequisites</span></span>
<span data-ttu-id="cef07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cef07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cef07-111">Permission type</span></span>|<span data-ttu-id="cef07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cef07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cef07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cef07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cef07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cef07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cef07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cef07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cef07-116">Not supported.</span></span>|
|<span data-ttu-id="cef07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cef07-117">Application</span></span>|<span data-ttu-id="cef07-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef07-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cef07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cef07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="cef07-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cef07-120">Request headers</span></span>
|<span data-ttu-id="cef07-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cef07-121">Header</span></span>|<span data-ttu-id="cef07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cef07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cef07-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cef07-123">Authorization</span></span>|<span data-ttu-id="cef07-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cef07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cef07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cef07-125">Accept</span></span>|<span data-ttu-id="cef07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cef07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef07-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cef07-127">Request body</span></span>
<span data-ttu-id="cef07-128">В тексте запроса добавьте представление объекта networkIPv6ConfigurationManagementCondition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cef07-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="cef07-129">В следующей таблице приведены свойства, необходимые при создании networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="cef07-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="cef07-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cef07-130">Property</span></span>|<span data-ttu-id="cef07-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cef07-131">Type</span></span>|<span data-ttu-id="cef07-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cef07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cef07-133">id</span><span class="sxs-lookup"><span data-stu-id="cef07-133">id</span></span>|<span data-ttu-id="cef07-134">String</span><span class="sxs-lookup"><span data-stu-id="cef07-134">String</span></span>|<span data-ttu-id="cef07-135">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="cef07-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="cef07-136">System generated value assigned when created.</span></span> <span data-ttu-id="cef07-137">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="cef07-138">uniqueName</span></span>|<span data-ttu-id="cef07-139">String</span><span class="sxs-lookup"><span data-stu-id="cef07-139">String</span></span>|<span data-ttu-id="cef07-140">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-140">Unique name for the management condition.</span></span> <span data-ttu-id="cef07-141">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-141">Used in management condition expressions.</span></span> <span data-ttu-id="cef07-142">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cef07-143">displayName</span></span>|<span data-ttu-id="cef07-144">Строка</span><span class="sxs-lookup"><span data-stu-id="cef07-144">String</span></span>|<span data-ttu-id="cef07-145">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="cef07-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="cef07-146">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-147">description</span><span class="sxs-lookup"><span data-stu-id="cef07-147">description</span></span>|<span data-ttu-id="cef07-148">String</span><span class="sxs-lookup"><span data-stu-id="cef07-148">String</span></span>|<span data-ttu-id="cef07-149">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="cef07-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="cef07-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cef07-151">createdDateTime</span></span>|<span data-ttu-id="cef07-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef07-152">DateTimeOffset</span></span>|<span data-ttu-id="cef07-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-153">The time the management condition was created.</span></span> <span data-ttu-id="cef07-154">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cef07-154">Generated service side.</span></span> <span data-ttu-id="cef07-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cef07-156">modifiedDateTime</span></span>|<span data-ttu-id="cef07-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef07-157">DateTimeOffset</span></span>|<span data-ttu-id="cef07-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-158">The time the management condition was last modified.</span></span> <span data-ttu-id="cef07-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cef07-159">Updated service side.</span></span> <span data-ttu-id="cef07-160">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-161">eTag</span><span class="sxs-lookup"><span data-stu-id="cef07-161">eTag</span></span>|<span data-ttu-id="cef07-162">String</span><span class="sxs-lookup"><span data-stu-id="cef07-162">String</span></span>|<span data-ttu-id="cef07-163">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-163">ETag of the management condition.</span></span> <span data-ttu-id="cef07-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="cef07-164">Updated service side.</span></span> <span data-ttu-id="cef07-165">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cef07-166">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="cef07-166">applicablePlatforms</span></span>|<span data-ttu-id="cef07-167">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="cef07-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cef07-168">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="cef07-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cef07-169">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="cef07-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="cef07-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cef07-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="cef07-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="cef07-171">ipV6Prefix</span></span>|<span data-ttu-id="cef07-172">String</span><span class="sxs-lookup"><span data-stu-id="cef07-172">String</span></span>|<span data-ttu-id="cef07-173">Подсеть IPv6, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="cef07-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="cef07-174">Например: 2001: db8::/32</span><span class="sxs-lookup"><span data-stu-id="cef07-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="cef07-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="cef07-175">ipV6Gateway</span></span>|<span data-ttu-id="cef07-176">String</span><span class="sxs-lookup"><span data-stu-id="cef07-176">String</span></span>|<span data-ttu-id="cef07-177">Адрес шлюза IPv6 в.</span><span class="sxs-lookup"><span data-stu-id="cef07-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="cef07-178">Например, 2001: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="cef07-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="cef07-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="cef07-179">ipV6DNSServerList</span></span>|<span data-ttu-id="cef07-180">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cef07-180">String collection</span></span>|<span data-ttu-id="cef07-181">DNS-серверы IPv6, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="cef07-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="cef07-182">днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="cef07-182">dnsSuffixList</span></span>|<span data-ttu-id="cef07-183">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cef07-183">String collection</span></span>|<span data-ttu-id="cef07-184">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="cef07-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="cef07-185">Например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="cef07-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="cef07-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="cef07-186">Response</span></span>
<span data-ttu-id="cef07-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cef07-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cef07-188">Пример</span><span class="sxs-lookup"><span data-stu-id="cef07-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="cef07-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="cef07-189">Request</span></span>
<span data-ttu-id="cef07-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cef07-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cef07-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="cef07-191">Response</span></span>
<span data-ttu-id="cef07-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cef07-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



