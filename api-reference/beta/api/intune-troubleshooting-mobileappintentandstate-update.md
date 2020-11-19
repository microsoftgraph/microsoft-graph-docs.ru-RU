---
title: Обновление Мобилеаппинтентандстате
description: Обновление свойств объекта Мобилеаппинтентандстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9934d3c1264b169574046d4ee86985d275325c9b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226876"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="c1191-103">Обновление Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="c1191-103">Update mobileAppIntentAndState</span></span>

<span data-ttu-id="c1191-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1191-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1191-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1191-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1191-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1191-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1191-107">Обновление свойств объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c1191-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1191-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1191-108">Prerequisites</span></span>
<span data-ttu-id="c1191-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1191-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1191-111">Permission type</span></span>|<span data-ttu-id="c1191-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1191-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1191-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1191-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1191-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c1191-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1191-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1191-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1191-116">Not supported.</span></span>|
|<span data-ttu-id="c1191-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1191-117">Application</span></span>|<span data-ttu-id="c1191-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1191-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1191-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1191-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c1191-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1191-120">Request headers</span></span>
|<span data-ttu-id="c1191-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1191-121">Header</span></span>|<span data-ttu-id="c1191-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1191-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1191-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1191-123">Authorization</span></span>|<span data-ttu-id="c1191-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1191-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1191-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1191-125">Accept</span></span>|<span data-ttu-id="c1191-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1191-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1191-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1191-127">Request body</span></span>
<span data-ttu-id="c1191-128">В тексте запроса добавьте представление объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1191-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="c1191-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="c1191-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="c1191-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1191-130">Property</span></span>|<span data-ttu-id="c1191-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1191-131">Type</span></span>|<span data-ttu-id="c1191-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1191-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1191-133">id</span><span class="sxs-lookup"><span data-stu-id="c1191-133">id</span></span>|<span data-ttu-id="c1191-134">String</span><span class="sxs-lookup"><span data-stu-id="c1191-134">String</span></span>|<span data-ttu-id="c1191-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c1191-135">UUID for the object</span></span>|
|<span data-ttu-id="c1191-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c1191-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="c1191-137">String</span><span class="sxs-lookup"><span data-stu-id="c1191-137">String</span></span>|<span data-ttu-id="c1191-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="c1191-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c1191-139">userId</span><span class="sxs-lookup"><span data-stu-id="c1191-139">userId</span></span>|<span data-ttu-id="c1191-140">String</span><span class="sxs-lookup"><span data-stu-id="c1191-140">String</span></span>|<span data-ttu-id="c1191-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="c1191-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c1191-142">мобилеапплист</span><span class="sxs-lookup"><span data-stu-id="c1191-142">mobileAppList</span></span>|<span data-ttu-id="c1191-143">Коллекция [мобилеаппинтентандстатедетаил](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)</span><span class="sxs-lookup"><span data-stu-id="c1191-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="c1191-144">Список целей и состояний полезных данных для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1191-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="c1191-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1191-145">Response</span></span>
<span data-ttu-id="c1191-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1191-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1191-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c1191-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1191-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1191-148">Request</span></span>
<span data-ttu-id="c1191-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1191-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1191-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1191-150">Response</span></span>
<span data-ttu-id="c1191-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1191-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




