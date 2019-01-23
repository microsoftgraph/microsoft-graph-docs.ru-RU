---
title: Обновление mobileAppIntentAndState
description: Обновление свойства объекта mobileAppIntentAndState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7157711819e4a5b3d4fbeb6ea6c8fce136da9380
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405193"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="de5ae-103">Обновление mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="de5ae-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="de5ae-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de5ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="de5ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de5ae-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de5ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de5ae-107">Обновление свойства объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="de5ae-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de5ae-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="de5ae-108">Prerequisites</span></span>
<span data-ttu-id="de5ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="de5ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="de5ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de5ae-111">Permission type</span></span>|<span data-ttu-id="de5ae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de5ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de5ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de5ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de5ae-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de5ae-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="de5ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de5ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de5ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5ae-116">Not supported.</span></span>|
|<span data-ttu-id="de5ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de5ae-117">Application</span></span>|<span data-ttu-id="de5ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de5ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de5ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="de5ae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de5ae-120">Request headers</span></span>
|<span data-ttu-id="de5ae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de5ae-121">Header</span></span>|<span data-ttu-id="de5ae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de5ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de5ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de5ae-123">Authorization</span></span>|<span data-ttu-id="de5ae-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="de5ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de5ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de5ae-125">Accept</span></span>|<span data-ttu-id="de5ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de5ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de5ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de5ae-127">Request body</span></span>
<span data-ttu-id="de5ae-128">В тексте запроса укажите представление JSON для объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="de5ae-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="de5ae-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="de5ae-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="de5ae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de5ae-130">Property</span></span>|<span data-ttu-id="de5ae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de5ae-131">Type</span></span>|<span data-ttu-id="de5ae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de5ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de5ae-133">id</span><span class="sxs-lookup"><span data-stu-id="de5ae-133">id</span></span>|<span data-ttu-id="de5ae-134">String</span><span class="sxs-lookup"><span data-stu-id="de5ae-134">String</span></span>|<span data-ttu-id="de5ae-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="de5ae-135">UUID for the object</span></span>|
|<span data-ttu-id="de5ae-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="de5ae-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="de5ae-137">String</span><span class="sxs-lookup"><span data-stu-id="de5ae-137">String</span></span>|<span data-ttu-id="de5ae-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="de5ae-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="de5ae-139">userId</span><span class="sxs-lookup"><span data-stu-id="de5ae-139">userId</span></span>|<span data-ttu-id="de5ae-140">String</span><span class="sxs-lookup"><span data-stu-id="de5ae-140">String</span></span>|<span data-ttu-id="de5ae-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="de5ae-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="de5ae-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="de5ae-142">mobileAppList</span></span>|<span data-ttu-id="de5ae-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="de5ae-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="de5ae-144">Список целей полезных данных и состояния для клиента.</span><span class="sxs-lookup"><span data-stu-id="de5ae-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="de5ae-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="de5ae-145">Response</span></span>
<span data-ttu-id="de5ae-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="de5ae-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de5ae-147">Пример</span><span class="sxs-lookup"><span data-stu-id="de5ae-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="de5ae-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="de5ae-148">Request</span></span>
<span data-ttu-id="de5ae-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de5ae-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de5ae-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="de5ae-150">Response</span></span>
<span data-ttu-id="de5ae-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="de5ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




