---
title: Создание Мобилеаппинтентандстате
description: Создание нового объекта Мобилеаппинтентандстате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6b5132675f09da3b26ffca6e51893ab64afed43
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800125"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="efb24-103">Создание Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="efb24-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="efb24-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efb24-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efb24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb24-106">Создание нового объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="efb24-106">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb24-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efb24-107">Prerequisites</span></span>
<span data-ttu-id="efb24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb24-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efb24-110">Permission type</span></span>|<span data-ttu-id="efb24-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efb24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb24-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efb24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efb24-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb24-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="efb24-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efb24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb24-115">Not supported.</span></span>|
|<span data-ttu-id="efb24-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="efb24-116">Application</span></span>|<span data-ttu-id="efb24-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb24-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb24-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efb24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="efb24-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efb24-119">Request headers</span></span>
|<span data-ttu-id="efb24-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efb24-120">Header</span></span>|<span data-ttu-id="efb24-121">Значение</span><span class="sxs-lookup"><span data-stu-id="efb24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb24-122">Authorization</span></span>|<span data-ttu-id="efb24-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efb24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb24-124">Accept</span><span class="sxs-lookup"><span data-stu-id="efb24-124">Accept</span></span>|<span data-ttu-id="efb24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efb24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb24-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efb24-126">Request body</span></span>
<span data-ttu-id="efb24-127">В тексте запроса добавьте представление объекта Мобилеаппинтентандстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efb24-127">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="efb24-128">В следующей таблице приведены свойства, необходимые при создании Мобилеаппинтентандстате.</span><span class="sxs-lookup"><span data-stu-id="efb24-128">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="efb24-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb24-129">Property</span></span>|<span data-ttu-id="efb24-130">Тип</span><span class="sxs-lookup"><span data-stu-id="efb24-130">Type</span></span>|<span data-ttu-id="efb24-131">Описание</span><span class="sxs-lookup"><span data-stu-id="efb24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb24-132">id</span><span class="sxs-lookup"><span data-stu-id="efb24-132">id</span></span>|<span data-ttu-id="efb24-133">Строка</span><span class="sxs-lookup"><span data-stu-id="efb24-133">String</span></span>|<span data-ttu-id="efb24-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="efb24-134">UUID for the object</span></span>|
|<span data-ttu-id="efb24-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="efb24-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="efb24-136">String</span><span class="sxs-lookup"><span data-stu-id="efb24-136">String</span></span>|<span data-ttu-id="efb24-137">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="efb24-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="efb24-138">userId</span><span class="sxs-lookup"><span data-stu-id="efb24-138">userId</span></span>|<span data-ttu-id="efb24-139">String</span><span class="sxs-lookup"><span data-stu-id="efb24-139">String</span></span>|<span data-ttu-id="efb24-140">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="efb24-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="efb24-141">мобилеапплист</span><span class="sxs-lookup"><span data-stu-id="efb24-141">mobileAppList</span></span>|<span data-ttu-id="efb24-142">Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="efb24-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="efb24-143">Список целей и состояний полезных данных для клиента.</span><span class="sxs-lookup"><span data-stu-id="efb24-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="efb24-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb24-144">Response</span></span>
<span data-ttu-id="efb24-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efb24-145">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb24-146">Пример</span><span class="sxs-lookup"><span data-stu-id="efb24-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb24-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="efb24-147">Request</span></span>
<span data-ttu-id="efb24-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efb24-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efb24-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb24-149">Response</span></span>
<span data-ttu-id="efb24-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efb24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




