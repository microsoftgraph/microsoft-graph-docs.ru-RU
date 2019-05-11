---
title: Создание Мобилеаппинтентандстате
description: Создание нового объекта Мобилеаппинтентандстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdf522608972a8a43d0b6fae2cef8e0afce65eff
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898703"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="a7916-103">Создание Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="a7916-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="a7916-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7916-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7916-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7916-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7916-106">Создание нового объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a7916-106">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7916-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7916-107">Prerequisites</span></span>
<span data-ttu-id="a7916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7916-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7916-110">Permission type</span></span>|<span data-ttu-id="a7916-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7916-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7916-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7916-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7916-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7916-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a7916-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7916-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7916-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7916-115">Not supported.</span></span>|
|<span data-ttu-id="a7916-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7916-116">Application</span></span>|<span data-ttu-id="a7916-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7916-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7916-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7916-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="a7916-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7916-119">Request headers</span></span>
|<span data-ttu-id="a7916-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7916-120">Header</span></span>|<span data-ttu-id="a7916-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a7916-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7916-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7916-122">Authorization</span></span>|<span data-ttu-id="a7916-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7916-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7916-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a7916-124">Accept</span></span>|<span data-ttu-id="a7916-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7916-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7916-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7916-126">Request body</span></span>
<span data-ttu-id="a7916-127">В тексте запроса добавьте представление объекта Мобилеаппинтентандстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7916-127">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="a7916-128">В следующей таблице приведены свойства, необходимые при создании Мобилеаппинтентандстате.</span><span class="sxs-lookup"><span data-stu-id="a7916-128">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="a7916-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7916-129">Property</span></span>|<span data-ttu-id="a7916-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a7916-130">Type</span></span>|<span data-ttu-id="a7916-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a7916-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7916-132">id</span><span class="sxs-lookup"><span data-stu-id="a7916-132">id</span></span>|<span data-ttu-id="a7916-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a7916-133">String</span></span>|<span data-ttu-id="a7916-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="a7916-134">UUID for the object</span></span>|
|<span data-ttu-id="a7916-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7916-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="a7916-136">String</span><span class="sxs-lookup"><span data-stu-id="a7916-136">String</span></span>|<span data-ttu-id="a7916-137">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="a7916-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a7916-138">userId</span><span class="sxs-lookup"><span data-stu-id="a7916-138">userId</span></span>|<span data-ttu-id="a7916-139">String</span><span class="sxs-lookup"><span data-stu-id="a7916-139">String</span></span>|<span data-ttu-id="a7916-140">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="a7916-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="a7916-141">Мобилеапплист</span><span class="sxs-lookup"><span data-stu-id="a7916-141">mobileAppList</span></span>|<span data-ttu-id="a7916-142">Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="a7916-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="a7916-143">Список целей и состояний полезных данных для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7916-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="a7916-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7916-144">Response</span></span>
<span data-ttu-id="a7916-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7916-145">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7916-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a7916-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7916-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7916-147">Request</span></span>
<span data-ttu-id="a7916-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7916-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7916-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7916-149">Response</span></span>
<span data-ttu-id="a7916-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7916-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




