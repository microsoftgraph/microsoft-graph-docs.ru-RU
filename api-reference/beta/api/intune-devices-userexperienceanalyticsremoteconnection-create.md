---
title: Создание userExperienceAnalyticsRemoteConnection
description: Создание нового объекта userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5937a7bc044ff56776242e3446a71ca5dd45cbac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446738"
---
# <a name="create-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="06c8e-103">Создание userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="06c8e-103">Create userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="06c8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06c8e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06c8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06c8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c8e-107">Создание нового [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="06c8e-107">Create a new [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06c8e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06c8e-108">Prerequisites</span></span>
<span data-ttu-id="06c8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06c8e-111">Permission type</span></span>|<span data-ttu-id="06c8e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06c8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c8e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06c8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06c8e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c8e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06c8e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06c8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c8e-116">Not supported.</span></span>|
|<span data-ttu-id="06c8e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="06c8e-117">Application</span></span>|<span data-ttu-id="06c8e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c8e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06c8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="06c8e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06c8e-120">Request headers</span></span>
|<span data-ttu-id="06c8e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06c8e-121">Header</span></span>|<span data-ttu-id="06c8e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06c8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c8e-123">Authorization</span></span>|<span data-ttu-id="06c8e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c8e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06c8e-125">Accept</span></span>|<span data-ttu-id="06c8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06c8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c8e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06c8e-127">Request body</span></span>
<span data-ttu-id="06c8e-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsRemoteConnection.</span><span class="sxs-lookup"><span data-stu-id="06c8e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsRemoteConnection object.</span></span>

<span data-ttu-id="06c8e-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsRemoteConnection.</span><span class="sxs-lookup"><span data-stu-id="06c8e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsRemoteConnection.</span></span>

|<span data-ttu-id="06c8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c8e-130">Property</span></span>|<span data-ttu-id="06c8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06c8e-131">Type</span></span>|<span data-ttu-id="06c8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06c8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c8e-133">id</span><span class="sxs-lookup"><span data-stu-id="06c8e-133">id</span></span>|<span data-ttu-id="06c8e-134">String</span><span class="sxs-lookup"><span data-stu-id="06c8e-134">String</span></span>|<span data-ttu-id="06c8e-135">Уникальный идентификатор объекта удаленного подключения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="06c8e-135">The unique identifier of the user experience analytics remote connection entity.</span></span>|
|<span data-ttu-id="06c8e-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="06c8e-136">deviceId</span></span>|<span data-ttu-id="06c8e-137">String</span><span class="sxs-lookup"><span data-stu-id="06c8e-137">String</span></span>|<span data-ttu-id="06c8e-138">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="06c8e-138">The id of the device.</span></span>|
|<span data-ttu-id="06c8e-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="06c8e-139">deviceName</span></span>|<span data-ttu-id="06c8e-140">String</span><span class="sxs-lookup"><span data-stu-id="06c8e-140">String</span></span>|<span data-ttu-id="06c8e-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="06c8e-141">The name of the device.</span></span>|
|<span data-ttu-id="06c8e-142">model</span><span class="sxs-lookup"><span data-stu-id="06c8e-142">model</span></span>|<span data-ttu-id="06c8e-143">String</span><span class="sxs-lookup"><span data-stu-id="06c8e-143">String</span></span>|<span data-ttu-id="06c8e-144">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="06c8e-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="06c8e-145">virtualNetwork</span><span class="sxs-lookup"><span data-stu-id="06c8e-145">virtualNetwork</span></span>|<span data-ttu-id="06c8e-146">String</span><span class="sxs-lookup"><span data-stu-id="06c8e-146">String</span></span>|<span data-ttu-id="06c8e-147">Виртуальная сеть аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="06c8e-147">The user experience analytics virtual network.</span></span>|
|<span data-ttu-id="06c8e-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="06c8e-148">deviceCount</span></span>|<span data-ttu-id="06c8e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="06c8e-149">Int32</span></span>|<span data-ttu-id="06c8e-150">Количество удаленных подключений.</span><span class="sxs-lookup"><span data-stu-id="06c8e-150">The count of remote connection.</span></span> <span data-ttu-id="06c8e-151">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="06c8e-151">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="06c8e-152">cloudPcRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="06c8e-152">cloudPcRoundTripTime</span></span>|<span data-ttu-id="06c8e-153">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-153">Double</span></span>|<span data-ttu-id="06c8e-154">Время круговой оконечности устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="06c8e-154">The round tip time of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-155">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="06c8e-155">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="06c8e-156">cloudPcSignInTime</span><span class="sxs-lookup"><span data-stu-id="06c8e-156">cloudPcSignInTime</span></span>|<span data-ttu-id="06c8e-157">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-157">Double</span></span>|<span data-ttu-id="06c8e-158">Вход во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="06c8e-158">The sign in time of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-159">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="06c8e-159">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="06c8e-160">remoteSignInTime</span><span class="sxs-lookup"><span data-stu-id="06c8e-160">remoteSignInTime</span></span>|<span data-ttu-id="06c8e-161">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-161">Double</span></span>|<span data-ttu-id="06c8e-162">Удаленный вход во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="06c8e-162">The remote sign in time of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-163">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="06c8e-163">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="06c8e-164">coreBootTime</span><span class="sxs-lookup"><span data-stu-id="06c8e-164">coreBootTime</span></span>|<span data-ttu-id="06c8e-165">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-165">Double</span></span>|<span data-ttu-id="06c8e-166">Основное время загрузки устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="06c8e-166">The core boot time of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-167">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="06c8e-167">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="06c8e-168">coreSignInTime</span><span class="sxs-lookup"><span data-stu-id="06c8e-168">coreSignInTime</span></span>|<span data-ttu-id="06c8e-169">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-169">Double</span></span>|<span data-ttu-id="06c8e-170">Основной знак во время устройства облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="06c8e-170">The core sign in time of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-171">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="06c8e-171">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="06c8e-172">cloudPcFailurePercentage</span><span class="sxs-lookup"><span data-stu-id="06c8e-172">cloudPcFailurePercentage</span></span>|<span data-ttu-id="06c8e-173">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="06c8e-173">Double</span></span>|<span data-ttu-id="06c8e-174">Вход в процент отказа облачного устройства PC.</span><span class="sxs-lookup"><span data-stu-id="06c8e-174">The sign in failure percentage of Cloud PC Device.</span></span> <span data-ttu-id="06c8e-175">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="06c8e-175">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="06c8e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="06c8e-176">Response</span></span>
<span data-ttu-id="06c8e-177">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06c8e-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c8e-178">Пример</span><span class="sxs-lookup"><span data-stu-id="06c8e-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="06c8e-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="06c8e-179">Request</span></span>
<span data-ttu-id="06c8e-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06c8e-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
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

### <a name="response"></a><span data-ttu-id="06c8e-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="06c8e-181">Response</span></span>
<span data-ttu-id="06c8e-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06c8e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




