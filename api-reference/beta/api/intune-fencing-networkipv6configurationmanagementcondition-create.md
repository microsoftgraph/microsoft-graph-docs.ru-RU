---
title: Создание networkIPv6ConfigurationManagementCondition
description: Создание нового объекта networkIPv6ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 454e80f66aaf1cc4421f719df522312b00df1be3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990220"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="861ec-103">Создание networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="861ec-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="861ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="861ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="861ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="861ec-106">Создание нового объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="861ec-106">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="861ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="861ec-107">Prerequisites</span></span>
<span data-ttu-id="861ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="861ec-110">Permission type</span></span>|<span data-ttu-id="861ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="861ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="861ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="861ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="861ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="861ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861ec-115">Not supported.</span></span>|
|<span data-ttu-id="861ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="861ec-116">Application</span></span>|<span data-ttu-id="861ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="861ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="861ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="861ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="861ec-119">Request headers</span></span>
|<span data-ttu-id="861ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="861ec-120">Header</span></span>|<span data-ttu-id="861ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="861ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="861ec-122">Authorization</span></span>|<span data-ttu-id="861ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="861ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="861ec-124">Accept</span></span>|<span data-ttu-id="861ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="861ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="861ec-126">Request body</span></span>
<span data-ttu-id="861ec-127">В тексте запроса добавьте представление объекта networkIPv6ConfigurationManagementCondition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="861ec-127">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="861ec-128">В следующей таблице приведены свойства, необходимые при создании networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="861ec-128">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="861ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="861ec-129">Property</span></span>|<span data-ttu-id="861ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="861ec-130">Type</span></span>|<span data-ttu-id="861ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="861ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861ec-132">id</span><span class="sxs-lookup"><span data-stu-id="861ec-132">id</span></span>|<span data-ttu-id="861ec-133">String</span><span class="sxs-lookup"><span data-stu-id="861ec-133">String</span></span>|<span data-ttu-id="861ec-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="861ec-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="861ec-135">System generated value assigned when created.</span></span> <span data-ttu-id="861ec-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="861ec-137">uniqueName</span></span>|<span data-ttu-id="861ec-138">String</span><span class="sxs-lookup"><span data-stu-id="861ec-138">String</span></span>|<span data-ttu-id="861ec-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-139">Unique name for the management condition.</span></span> <span data-ttu-id="861ec-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-140">Used in management condition expressions.</span></span> <span data-ttu-id="861ec-141">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-142">displayName</span><span class="sxs-lookup"><span data-stu-id="861ec-142">displayName</span></span>|<span data-ttu-id="861ec-143">Строка</span><span class="sxs-lookup"><span data-stu-id="861ec-143">String</span></span>|<span data-ttu-id="861ec-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="861ec-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="861ec-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-146">description</span><span class="sxs-lookup"><span data-stu-id="861ec-146">description</span></span>|<span data-ttu-id="861ec-147">String</span><span class="sxs-lookup"><span data-stu-id="861ec-147">String</span></span>|<span data-ttu-id="861ec-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="861ec-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="861ec-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="861ec-150">createdDateTime</span></span>|<span data-ttu-id="861ec-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861ec-151">DateTimeOffset</span></span>|<span data-ttu-id="861ec-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-152">The time the management condition was created.</span></span> <span data-ttu-id="861ec-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="861ec-153">Generated service side.</span></span> <span data-ttu-id="861ec-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="861ec-155">modifiedDateTime</span></span>|<span data-ttu-id="861ec-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861ec-156">DateTimeOffset</span></span>|<span data-ttu-id="861ec-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-157">The time the management condition was last modified.</span></span> <span data-ttu-id="861ec-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="861ec-158">Updated service side.</span></span> <span data-ttu-id="861ec-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-160">eTag</span><span class="sxs-lookup"><span data-stu-id="861ec-160">eTag</span></span>|<span data-ttu-id="861ec-161">String</span><span class="sxs-lookup"><span data-stu-id="861ec-161">String</span></span>|<span data-ttu-id="861ec-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-162">ETag of the management condition.</span></span> <span data-ttu-id="861ec-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="861ec-163">Updated service side.</span></span> <span data-ttu-id="861ec-164">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="861ec-165">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="861ec-165">applicablePlatforms</span></span>|<span data-ttu-id="861ec-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="861ec-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="861ec-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="861ec-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="861ec-168">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="861ec-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="861ec-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="861ec-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="861ec-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="861ec-170">ipV6Prefix</span></span>|<span data-ttu-id="861ec-171">String</span><span class="sxs-lookup"><span data-stu-id="861ec-171">String</span></span>|<span data-ttu-id="861ec-172">Подсеть IPv6, к которой необходимо подключиться.</span><span class="sxs-lookup"><span data-stu-id="861ec-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="861ec-173">Например: 2001: db8::/32</span><span class="sxs-lookup"><span data-stu-id="861ec-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="861ec-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="861ec-174">ipV6Gateway</span></span>|<span data-ttu-id="861ec-175">String</span><span class="sxs-lookup"><span data-stu-id="861ec-175">String</span></span>|<span data-ttu-id="861ec-176">Адрес шлюза IPv6 в.</span><span class="sxs-lookup"><span data-stu-id="861ec-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="861ec-177">Например, 2001: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="861ec-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="861ec-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="861ec-178">ipV6DNSServerList</span></span>|<span data-ttu-id="861ec-179">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="861ec-179">String collection</span></span>|<span data-ttu-id="861ec-180">DNS-серверы IPv6, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="861ec-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="861ec-181">Днссуффикслист</span><span class="sxs-lookup"><span data-stu-id="861ec-181">dnsSuffixList</span></span>|<span data-ttu-id="861ec-182">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="861ec-182">String collection</span></span>|<span data-ttu-id="861ec-183">Допустимые DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="861ec-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="861ec-184">Например, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="861ec-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="861ec-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="861ec-185">Response</span></span>
<span data-ttu-id="861ec-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="861ec-186">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861ec-187">Пример</span><span class="sxs-lookup"><span data-stu-id="861ec-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="861ec-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="861ec-188">Request</span></span>
<span data-ttu-id="861ec-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="861ec-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="861ec-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="861ec-190">Response</span></span>
<span data-ttu-id="861ec-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="861ec-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





