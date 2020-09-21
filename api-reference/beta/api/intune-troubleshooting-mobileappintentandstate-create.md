---
title: Создание Мобилеаппинтентандстате
description: Создание нового объекта Мобилеаппинтентандстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 985008e7b4680f36bd2aa0c669bdc8a3912dda88
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966900"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="f4767-103">Создание Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="f4767-103">Create mobileAppIntentAndState</span></span>

<span data-ttu-id="f4767-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4767-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4767-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4767-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4767-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4767-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4767-107">Создание нового объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f4767-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4767-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4767-108">Prerequisites</span></span>
<span data-ttu-id="f4767-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4767-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4767-111">Permission type</span></span>|<span data-ttu-id="f4767-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4767-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4767-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4767-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4767-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4767-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4767-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4767-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4767-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4767-116">Not supported.</span></span>|
|<span data-ttu-id="f4767-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4767-117">Application</span></span>|<span data-ttu-id="f4767-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4767-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4767-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4767-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="f4767-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4767-120">Request headers</span></span>
|<span data-ttu-id="f4767-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4767-121">Header</span></span>|<span data-ttu-id="f4767-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4767-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4767-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4767-123">Authorization</span></span>|<span data-ttu-id="f4767-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4767-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4767-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4767-125">Accept</span></span>|<span data-ttu-id="f4767-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4767-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4767-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4767-127">Request body</span></span>
<span data-ttu-id="f4767-128">В тексте запроса добавьте представление объекта Мобилеаппинтентандстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4767-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="f4767-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппинтентандстате.</span><span class="sxs-lookup"><span data-stu-id="f4767-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="f4767-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4767-130">Property</span></span>|<span data-ttu-id="f4767-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4767-131">Type</span></span>|<span data-ttu-id="f4767-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4767-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4767-133">id</span><span class="sxs-lookup"><span data-stu-id="f4767-133">id</span></span>|<span data-ttu-id="f4767-134">String</span><span class="sxs-lookup"><span data-stu-id="f4767-134">String</span></span>|<span data-ttu-id="f4767-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="f4767-135">UUID for the object</span></span>|
|<span data-ttu-id="f4767-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4767-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="f4767-137">String</span><span class="sxs-lookup"><span data-stu-id="f4767-137">String</span></span>|<span data-ttu-id="f4767-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="f4767-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f4767-139">userId</span><span class="sxs-lookup"><span data-stu-id="f4767-139">userId</span></span>|<span data-ttu-id="f4767-140">String</span><span class="sxs-lookup"><span data-stu-id="f4767-140">String</span></span>|<span data-ttu-id="f4767-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="f4767-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f4767-142">мобилеапплист</span><span class="sxs-lookup"><span data-stu-id="f4767-142">mobileAppList</span></span>|<span data-ttu-id="f4767-143">Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="f4767-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="f4767-144">Список целей и состояний полезных данных для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4767-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="f4767-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4767-145">Response</span></span>
<span data-ttu-id="f4767-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4767-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4767-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f4767-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4767-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4767-148">Request</span></span>
<span data-ttu-id="f4767-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4767-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
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

### <a name="response"></a><span data-ttu-id="f4767-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4767-150">Response</span></span>
<span data-ttu-id="f4767-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4767-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






