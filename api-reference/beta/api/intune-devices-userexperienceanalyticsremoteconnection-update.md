---
title: Обновление userExperienceAnalyticsRemoteConnection
description: Обновление свойств объекта userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6287f070f0bbd610bab40694d3c41fcb6e701a7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446732"
---
# <a name="update-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="a5bd3-103">Обновление userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="a5bd3-103">Update userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="a5bd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5bd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5bd3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5bd3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5bd3-107">Обновление свойств объекта [userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-107">Update the properties of a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5bd3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a5bd3-108">Prerequisites</span></span>
<span data-ttu-id="a5bd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5bd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5bd3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5bd3-111">Permission type</span></span>|<span data-ttu-id="a5bd3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5bd3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5bd3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bd3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a5bd3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5bd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-116">Not supported.</span></span>|
|<span data-ttu-id="a5bd3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5bd3-117">Application</span></span>|<span data-ttu-id="a5bd3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bd3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5bd3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5bd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="request-headers"></a><span data-ttu-id="a5bd3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5bd3-120">Request headers</span></span>
|<span data-ttu-id="a5bd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5bd3-121">Header</span></span>|<span data-ttu-id="a5bd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5bd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5bd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5bd3-123">Authorization</span></span>|<span data-ttu-id="a5bd3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5bd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5bd3-125">Accept</span></span>|<span data-ttu-id="a5bd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5bd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5bd3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5bd3-127">Request body</span></span>
<span data-ttu-id="a5bd3-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

<span data-ttu-id="a5bd3-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="a5bd3-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).</span></span>

|<span data-ttu-id="a5bd3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5bd3-130">Property</span></span>|<span data-ttu-id="a5bd3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5bd3-131">Type</span></span>|<span data-ttu-id="a5bd3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5bd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5bd3-133">id</span><span class="sxs-lookup"><span data-stu-id="a5bd3-133">id</span></span>|<span data-ttu-id="a5bd3-134">String</span><span class="sxs-lookup"><span data-stu-id="a5bd3-134">String</span></span>|<span data-ttu-id="a5bd3-135">Уникальный идентификатор объекта удаленного подключения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-135">The unique identifier of the user experience analytics remote connection entity.</span></span>|
|<span data-ttu-id="a5bd3-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="a5bd3-136">deviceId</span></span>|<span data-ttu-id="a5bd3-137">String</span><span class="sxs-lookup"><span data-stu-id="a5bd3-137">String</span></span>|<span data-ttu-id="a5bd3-138">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-138">The id of the device.</span></span>|
|<span data-ttu-id="a5bd3-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="a5bd3-139">deviceName</span></span>|<span data-ttu-id="a5bd3-140">String</span><span class="sxs-lookup"><span data-stu-id="a5bd3-140">String</span></span>|<span data-ttu-id="a5bd3-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-141">The name of the device.</span></span>|
|<span data-ttu-id="a5bd3-142">model</span><span class="sxs-lookup"><span data-stu-id="a5bd3-142">model</span></span>|<span data-ttu-id="a5bd3-143">String</span><span class="sxs-lookup"><span data-stu-id="a5bd3-143">String</span></span>|<span data-ttu-id="a5bd3-144">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="a5bd3-145">virtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a5bd3-145">virtualNetwork</span></span>|<span data-ttu-id="a5bd3-146">String</span><span class="sxs-lookup"><span data-stu-id="a5bd3-146">String</span></span>|<span data-ttu-id="a5bd3-147">Виртуальная сеть аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-147">The user experience analytics virtual network.</span></span>|
|<span data-ttu-id="a5bd3-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a5bd3-148">deviceCount</span></span>|<span data-ttu-id="a5bd3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a5bd3-149">Int32</span></span>|<span data-ttu-id="a5bd3-150">Количество удаленных подключений.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-150">The count of remote connection.</span></span> <span data-ttu-id="a5bd3-151">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5bd3-151">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="a5bd3-152">cloudPcRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="a5bd3-152">cloudPcRoundTripTime</span></span>|<span data-ttu-id="a5bd3-153">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-153">Double</span></span>|<span data-ttu-id="a5bd3-154">Время круговой оконечности устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-154">The round tip time of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-155">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="a5bd3-155">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a5bd3-156">cloudPcSignInTime</span><span class="sxs-lookup"><span data-stu-id="a5bd3-156">cloudPcSignInTime</span></span>|<span data-ttu-id="a5bd3-157">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-157">Double</span></span>|<span data-ttu-id="a5bd3-158">Вход во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-158">The sign in time of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-159">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="a5bd3-159">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a5bd3-160">remoteSignInTime</span><span class="sxs-lookup"><span data-stu-id="a5bd3-160">remoteSignInTime</span></span>|<span data-ttu-id="a5bd3-161">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-161">Double</span></span>|<span data-ttu-id="a5bd3-162">Удаленный вход во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-162">The remote sign in time of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-163">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="a5bd3-163">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a5bd3-164">coreBootTime</span><span class="sxs-lookup"><span data-stu-id="a5bd3-164">coreBootTime</span></span>|<span data-ttu-id="a5bd3-165">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-165">Double</span></span>|<span data-ttu-id="a5bd3-166">Основное время загрузки устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-166">The core boot time of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-167">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="a5bd3-167">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a5bd3-168">coreSignInTime</span><span class="sxs-lookup"><span data-stu-id="a5bd3-168">coreSignInTime</span></span>|<span data-ttu-id="a5bd3-169">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-169">Double</span></span>|<span data-ttu-id="a5bd3-170">Основной знак во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-170">The core sign in time of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-171">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="a5bd3-171">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a5bd3-172">cloudPcFailurePercentage</span><span class="sxs-lookup"><span data-stu-id="a5bd3-172">cloudPcFailurePercentage</span></span>|<span data-ttu-id="a5bd3-173">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a5bd3-173">Double</span></span>|<span data-ttu-id="a5bd3-174">Вход в процент отказа облачного устройства PC.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-174">The sign in failure percentage of Cloud PC Device.</span></span> <span data-ttu-id="a5bd3-175">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="a5bd3-175">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="a5bd3-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5bd3-176">Response</span></span>
<span data-ttu-id="a5bd3-177">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5bd3-178">Пример</span><span class="sxs-lookup"><span data-stu-id="a5bd3-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5bd3-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5bd3-179">Request</span></span>
<span data-ttu-id="a5bd3-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```

### <a name="response"></a><span data-ttu-id="a5bd3-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5bd3-181">Response</span></span>
<span data-ttu-id="a5bd3-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5bd3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```




