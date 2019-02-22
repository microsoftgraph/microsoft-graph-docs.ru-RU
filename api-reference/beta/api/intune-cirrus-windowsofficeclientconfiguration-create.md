---
title: Создание Виндовсоффицеклиентконфигуратион
description: Создайте новую политику, не являющуюся политикой безопасности, с целевыми группами.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5a8e11fcf9728a554c8938d3ccf2314bf5e1999c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164164"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="86a34-103">Создание Виндовсоффицеклиентконфигуратион</span><span class="sxs-lookup"><span data-stu-id="86a34-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="86a34-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a34-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86a34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a34-106">Создайте новую политику, не являющуюся политикой безопасности, с целевыми группами.</span><span class="sxs-lookup"><span data-stu-id="86a34-106">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a34-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86a34-107">Prerequisites</span></span>
<span data-ttu-id="86a34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a34-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86a34-110">Permission type</span></span>|<span data-ttu-id="86a34-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86a34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a34-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86a34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a34-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a34-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86a34-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86a34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a34-115">Not supported.</span></span>|
|<span data-ttu-id="86a34-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86a34-116">Application</span></span>|<span data-ttu-id="86a34-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a34-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86a34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86a34-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86a34-119">Request headers</span></span>
|<span data-ttu-id="86a34-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86a34-120">Header</span></span>|<span data-ttu-id="86a34-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86a34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a34-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86a34-122">Authorization</span></span>|<span data-ttu-id="86a34-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="86a34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a34-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86a34-124">Accept</span></span>|<span data-ttu-id="86a34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86a34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a34-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86a34-126">Request body</span></span>
<span data-ttu-id="86a34-127">В тексте запроса добавьте представление объекта [Виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86a34-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="86a34-128">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a34-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="86a34-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="86a34-129">Property</span></span>|<span data-ttu-id="86a34-130">Тип</span><span class="sxs-lookup"><span data-stu-id="86a34-130">Type</span></span>|<span data-ttu-id="86a34-131">Описание</span><span class="sxs-lookup"><span data-stu-id="86a34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a34-132">id</span><span class="sxs-lookup"><span data-stu-id="86a34-132">id</span></span>|<span data-ttu-id="86a34-133">String</span><span class="sxs-lookup"><span data-stu-id="86a34-133">String</span></span>|<span data-ttu-id="86a34-134">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="86a34-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="86a34-135">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-136">Усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="86a34-136">userPreferencePayload</span></span>|<span data-ttu-id="86a34-137">Stream</span><span class="sxs-lookup"><span data-stu-id="86a34-137">Stream</span></span>|<span data-ttu-id="86a34-138">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="86a34-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="86a34-139">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-140">Полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="86a34-140">policyPayload</span></span>|<span data-ttu-id="86a34-141">Stream</span><span class="sxs-lookup"><span data-stu-id="86a34-141">Stream</span></span>|<span data-ttu-id="86a34-142">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="86a34-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="86a34-143">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-144">description</span><span class="sxs-lookup"><span data-stu-id="86a34-144">description</span></span>|<span data-ttu-id="86a34-145">String</span><span class="sxs-lookup"><span data-stu-id="86a34-145">String</span></span>|<span data-ttu-id="86a34-146">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="86a34-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="86a34-147">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-148">displayName</span><span class="sxs-lookup"><span data-stu-id="86a34-148">displayName</span></span>|<span data-ttu-id="86a34-149">String</span><span class="sxs-lookup"><span data-stu-id="86a34-149">String</span></span>|<span data-ttu-id="86a34-150">Предоставленное администратором имя политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="86a34-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="86a34-151">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-152">assignments</span><span class="sxs-lookup"><span data-stu-id="86a34-152">assignments</span></span>|<span data-ttu-id="86a34-153">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="86a34-154">Список назначений групп для политики..</span><span class="sxs-lookup"><span data-stu-id="86a34-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="86a34-155">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-156">priority</span><span class="sxs-lookup"><span data-stu-id="86a34-156">priority</span></span>|<span data-ttu-id="86a34-157">Int32</span><span class="sxs-lookup"><span data-stu-id="86a34-157">Int32</span></span>|<span data-ttu-id="86a34-158">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="86a34-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="86a34-159">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86a34-160">lastModifiedDateTime</span></span>|<span data-ttu-id="86a34-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="86a34-161">DateTime</span></span>|<span data-ttu-id="86a34-162">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="86a34-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="86a34-163">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-164">Усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="86a34-164">userCheckinSummary</span></span>|[<span data-ttu-id="86a34-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="86a34-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="86a34-166">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="86a34-166">User check-in summary for the policy.</span></span> <span data-ttu-id="86a34-167">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="86a34-168">Чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="86a34-168">checkinStatuses</span></span>|<span data-ttu-id="86a34-169">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="86a34-170">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="86a34-170">List of office Client check-in status.</span></span> <span data-ttu-id="86a34-171">НаСледуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a34-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="86a34-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a34-172">Response</span></span>
<span data-ttu-id="86a34-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86a34-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a34-174">Пример</span><span class="sxs-lookup"><span data-stu-id="86a34-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a34-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="86a34-175">Request</span></span>
<span data-ttu-id="86a34-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86a34-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="86a34-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a34-177">Response</span></span>
<span data-ttu-id="86a34-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86a34-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```



