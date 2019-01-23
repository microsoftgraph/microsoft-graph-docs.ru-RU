---
title: Создание windowsOfficeClientConfiguration
description: Создайте новую политику не безопасности при указании на группы.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a915447ad22438d021bb4577fc856bbe89db1fdc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394378"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="98b79-103">Создание windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="98b79-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="98b79-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98b79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98b79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98b79-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98b79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b79-107">Создайте новую политику не безопасности при указании на группы.</span><span class="sxs-lookup"><span data-stu-id="98b79-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98b79-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="98b79-108">Prerequisites</span></span>
<span data-ttu-id="98b79-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98b79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98b79-111">Permission type</span></span>|<span data-ttu-id="98b79-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98b79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98b79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98b79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98b79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98b79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98b79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98b79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b79-116">Not supported.</span></span>|
|<span data-ttu-id="98b79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98b79-117">Application</span></span>|<span data-ttu-id="98b79-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98b79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98b79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="98b79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98b79-120">Request headers</span></span>
|<span data-ttu-id="98b79-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98b79-121">Header</span></span>|<span data-ttu-id="98b79-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98b79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98b79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98b79-123">Authorization</span></span>|<span data-ttu-id="98b79-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="98b79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98b79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98b79-125">Accept</span></span>|<span data-ttu-id="98b79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98b79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98b79-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98b79-127">Request body</span></span>
<span data-ttu-id="98b79-128">В тексте запроса укажите представление JSON для объекта [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="98b79-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="98b79-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98b79-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="98b79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b79-130">Property</span></span>|<span data-ttu-id="98b79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98b79-131">Type</span></span>|<span data-ttu-id="98b79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98b79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b79-133">id</span><span class="sxs-lookup"><span data-stu-id="98b79-133">id</span></span>|<span data-ttu-id="98b79-134">String</span><span class="sxs-lookup"><span data-stu-id="98b79-134">String</span></span>|<span data-ttu-id="98b79-135">Идентификатор политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="98b79-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="98b79-136">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="98b79-137">userPreferencePayload</span></span>|<span data-ttu-id="98b79-138">Stream</span><span class="sxs-lookup"><span data-stu-id="98b79-138">Stream</span></span>|<span data-ttu-id="98b79-139">Строка настройки JSON в двоичном формате, эти значения можно переопределить пользователем.</span><span class="sxs-lookup"><span data-stu-id="98b79-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="98b79-140">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="98b79-141">policyPayload</span></span>|<span data-ttu-id="98b79-142">Stream</span><span class="sxs-lookup"><span data-stu-id="98b79-142">Stream</span></span>|<span data-ttu-id="98b79-143">Параметры политики JSON string в двоичном формате, пользователь не может изменить эти значения.</span><span class="sxs-lookup"><span data-stu-id="98b79-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="98b79-144">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-145">description</span><span class="sxs-lookup"><span data-stu-id="98b79-145">description</span></span>|<span data-ttu-id="98b79-146">String</span><span class="sxs-lookup"><span data-stu-id="98b79-146">String</span></span>|<span data-ttu-id="98b79-147">Admin предоставляются описание клиента office конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="98b79-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="98b79-148">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-149">displayName</span><span class="sxs-lookup"><span data-stu-id="98b79-149">displayName</span></span>|<span data-ttu-id="98b79-150">String</span><span class="sxs-lookup"><span data-stu-id="98b79-150">String</span></span>|<span data-ttu-id="98b79-151">Admin предоставлено имя политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="98b79-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="98b79-152">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-153">assignments</span><span class="sxs-lookup"><span data-stu-id="98b79-153">assignments</span></span>|<span data-ttu-id="98b79-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="98b79-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="98b79-155">Список назначений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="98b79-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="98b79-156">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-157">priority</span><span class="sxs-lookup"><span data-stu-id="98b79-157">priority</span></span>|<span data-ttu-id="98b79-158">Int32</span><span class="sxs-lookup"><span data-stu-id="98b79-158">Int32</span></span>|<span data-ttu-id="98b79-159">Значение приоритета должно быть уникальное значение для каждой политики в области клиента и будет использоваться для разрешения конфликтов, меньшее значение означает, что высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="98b79-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="98b79-160">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98b79-161">lastModifiedDateTime</span></span>|<span data-ttu-id="98b79-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="98b79-162">DateTime</span></span>|<span data-ttu-id="98b79-163">Отметка измененные даты и времени последнего политики.</span><span class="sxs-lookup"><span data-stu-id="98b79-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="98b79-164">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="98b79-165">userCheckinSummary</span></span>|[<span data-ttu-id="98b79-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="98b79-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="98b79-167">Возврат Сводка пользователей для политики.</span><span class="sxs-lookup"><span data-stu-id="98b79-167">User check-in summary for the policy.</span></span> <span data-ttu-id="98b79-168">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="98b79-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="98b79-169">checkinStatuses</span></span>|<span data-ttu-id="98b79-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="98b79-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="98b79-171">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="98b79-171">List of office Client check-in status.</span></span> <span data-ttu-id="98b79-172">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98b79-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="98b79-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="98b79-173">Response</span></span>
<span data-ttu-id="98b79-174">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98b79-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b79-175">Пример</span><span class="sxs-lookup"><span data-stu-id="98b79-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="98b79-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="98b79-176">Request</span></span>
<span data-ttu-id="98b79-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98b79-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98b79-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="98b79-178">Response</span></span>
<span data-ttu-id="98b79-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="98b79-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



