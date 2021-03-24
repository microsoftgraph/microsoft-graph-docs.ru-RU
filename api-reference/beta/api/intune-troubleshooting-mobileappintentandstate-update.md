---
title: Обновление mobileAppIntentAndState
description: Обновление свойств объекта mobileAppIntentAndState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65a2076469d01891f889d1b4df11ba8ad1e2b445
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141493"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="fbd76-103">Обновление mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="fbd76-103">Update mobileAppIntentAndState</span></span>

<span data-ttu-id="fbd76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbd76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbd76-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbd76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbd76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbd76-107">Обновление свойств объекта [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)</span><span class="sxs-lookup"><span data-stu-id="fbd76-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbd76-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fbd76-108">Prerequisites</span></span>
<span data-ttu-id="fbd76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd76-111">Permission type</span></span>|<span data-ttu-id="fbd76-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbd76-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbd76-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbd76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd76-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd76-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fbd76-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbd76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbd76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd76-116">Not supported.</span></span>|
|<span data-ttu-id="fbd76-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fbd76-117">Application</span></span>|<span data-ttu-id="fbd76-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd76-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbd76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbd76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="fbd76-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbd76-120">Request headers</span></span>
|<span data-ttu-id="fbd76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbd76-121">Header</span></span>|<span data-ttu-id="fbd76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbd76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbd76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd76-123">Authorization</span></span>|<span data-ttu-id="fbd76-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbd76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbd76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbd76-125">Accept</span></span>|<span data-ttu-id="fbd76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd76-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbd76-127">Request body</span></span>
<span data-ttu-id="fbd76-128">В теле запроса поставляем представление JSON для [объекта mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)</span><span class="sxs-lookup"><span data-stu-id="fbd76-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="fbd76-129">В следующей таблице показаны свойства, необходимые при создании [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)</span><span class="sxs-lookup"><span data-stu-id="fbd76-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="fbd76-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbd76-130">Property</span></span>|<span data-ttu-id="fbd76-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbd76-131">Type</span></span>|<span data-ttu-id="fbd76-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbd76-133">id</span><span class="sxs-lookup"><span data-stu-id="fbd76-133">id</span></span>|<span data-ttu-id="fbd76-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd76-134">String</span></span>|<span data-ttu-id="fbd76-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="fbd76-135">UUID for the object</span></span>|
|<span data-ttu-id="fbd76-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fbd76-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="fbd76-137">String</span><span class="sxs-lookup"><span data-stu-id="fbd76-137">String</span></span>|<span data-ttu-id="fbd76-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="fbd76-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="fbd76-139">userId</span><span class="sxs-lookup"><span data-stu-id="fbd76-139">userId</span></span>|<span data-ttu-id="fbd76-140">String</span><span class="sxs-lookup"><span data-stu-id="fbd76-140">String</span></span>|<span data-ttu-id="fbd76-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="fbd76-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="fbd76-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="fbd76-142">mobileAppList</span></span>|<span data-ttu-id="fbd76-143">[коллекция mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="fbd76-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="fbd76-144">Список намерений и состояния полезной нагрузки для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbd76-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="fbd76-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbd76-145">Response</span></span>
<span data-ttu-id="fbd76-146">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbd76-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd76-147">Пример</span><span class="sxs-lookup"><span data-stu-id="fbd76-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbd76-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbd76-148">Request</span></span>
<span data-ttu-id="fbd76-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbd76-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fbd76-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbd76-150">Response</span></span>
<span data-ttu-id="fbd76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbd76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```




