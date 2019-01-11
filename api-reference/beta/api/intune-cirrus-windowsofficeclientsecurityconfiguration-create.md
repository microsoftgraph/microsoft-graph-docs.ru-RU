---
title: Создание windowsOfficeClientSecurityConfiguration
description: Создание нового объекта windowsOfficeClientSecurityConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 930d12432ec4b21e2293f1ded48a0a07625734cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837123"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="542d4-103">Создание windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="542d4-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="542d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="542d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="542d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="542d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="542d4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="542d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="542d4-107">Создание нового объекта [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="542d4-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="542d4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="542d4-108">Prerequisites</span></span>
<span data-ttu-id="542d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="542d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="542d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="542d4-111">Permission type</span></span>|<span data-ttu-id="542d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="542d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="542d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="542d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="542d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="542d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="542d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="542d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="542d4-116">Not supported.</span></span>|
|<span data-ttu-id="542d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="542d4-117">Application</span></span>|<span data-ttu-id="542d4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="542d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="542d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="542d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="542d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="542d4-120">Request headers</span></span>
|<span data-ttu-id="542d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="542d4-121">Header</span></span>|<span data-ttu-id="542d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="542d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="542d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="542d4-123">Authorization</span></span>|<span data-ttu-id="542d4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="542d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="542d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="542d4-125">Accept</span></span>|<span data-ttu-id="542d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="542d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="542d4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="542d4-127">Request body</span></span>
<span data-ttu-id="542d4-128">В тексте запроса укажите представление JSON для объекта [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="542d4-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="542d4-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="542d4-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="542d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="542d4-130">Property</span></span>|<span data-ttu-id="542d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="542d4-131">Type</span></span>|<span data-ttu-id="542d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="542d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542d4-133">id</span><span class="sxs-lookup"><span data-stu-id="542d4-133">id</span></span>|<span data-ttu-id="542d4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="542d4-134">String</span></span>|<span data-ttu-id="542d4-135">Идентификатор политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="542d4-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="542d4-136">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="542d4-137">userPreferencePayload</span></span>|<span data-ttu-id="542d4-138">Stream</span><span class="sxs-lookup"><span data-stu-id="542d4-138">Stream</span></span>|<span data-ttu-id="542d4-139">Строка настройки JSON в двоичном формате, эти значения можно переопределить пользователем.</span><span class="sxs-lookup"><span data-stu-id="542d4-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="542d4-140">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="542d4-141">policyPayload</span></span>|<span data-ttu-id="542d4-142">Stream</span><span class="sxs-lookup"><span data-stu-id="542d4-142">Stream</span></span>|<span data-ttu-id="542d4-143">Параметры политики JSON string в двоичном формате, пользователь не может изменить эти значения.</span><span class="sxs-lookup"><span data-stu-id="542d4-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="542d4-144">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-145">описание</span><span class="sxs-lookup"><span data-stu-id="542d4-145">description</span></span>|<span data-ttu-id="542d4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="542d4-146">String</span></span>|<span data-ttu-id="542d4-147">Admin предоставляются описание клиента office конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="542d4-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="542d4-148">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-149">displayName</span><span class="sxs-lookup"><span data-stu-id="542d4-149">displayName</span></span>|<span data-ttu-id="542d4-150">Строка</span><span class="sxs-lookup"><span data-stu-id="542d4-150">String</span></span>|<span data-ttu-id="542d4-151">Admin предоставлено имя политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="542d4-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="542d4-152">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-153">assignments</span><span class="sxs-lookup"><span data-stu-id="542d4-153">assignments</span></span>|<span data-ttu-id="542d4-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="542d4-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="542d4-155">Список назначений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="542d4-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="542d4-156">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-157">priority</span><span class="sxs-lookup"><span data-stu-id="542d4-157">priority</span></span>|<span data-ttu-id="542d4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="542d4-158">Int32</span></span>|<span data-ttu-id="542d4-159">Значение приоритета должно быть уникальное значение для каждой политики в области клиента и будет использоваться для разрешения конфликтов, меньшее значение означает, что высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="542d4-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="542d4-160">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="542d4-161">lastModifiedDateTime</span></span>|<span data-ttu-id="542d4-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="542d4-162">DateTime</span></span>|<span data-ttu-id="542d4-163">Отметка измененные даты и времени последнего политики.</span><span class="sxs-lookup"><span data-stu-id="542d4-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="542d4-164">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="542d4-165">userCheckinSummary</span></span>|[<span data-ttu-id="542d4-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="542d4-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="542d4-167">Возврат Сводка пользователей для политики.</span><span class="sxs-lookup"><span data-stu-id="542d4-167">User check-in summary for the policy.</span></span> <span data-ttu-id="542d4-168">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="542d4-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="542d4-169">checkinStatuses</span></span>|<span data-ttu-id="542d4-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="542d4-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="542d4-171">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="542d4-171">List of office Client check-in status.</span></span> <span data-ttu-id="542d4-172">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542d4-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="542d4-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="542d4-173">Response</span></span>
<span data-ttu-id="542d4-174">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="542d4-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="542d4-175">Пример</span><span class="sxs-lookup"><span data-stu-id="542d4-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="542d4-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="542d4-176">Request</span></span>
<span data-ttu-id="542d4-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="542d4-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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

### <a name="response"></a><span data-ttu-id="542d4-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="542d4-178">Response</span></span>
<span data-ttu-id="542d4-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="542d4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



