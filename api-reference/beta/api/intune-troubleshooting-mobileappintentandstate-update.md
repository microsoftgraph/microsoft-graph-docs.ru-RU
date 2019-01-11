---
title: Обновление mobileAppIntentAndState
description: Обновление свойства объекта mobileAppIntentAndState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd43c13d8e166563e60cb36cdcad980e25124aa5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827099"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="bcdb3-103">Обновление mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="bcdb3-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="bcdb3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcdb3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcdb3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcdb3-107">Обновление свойства объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bcdb3-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcdb3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcdb3-108">Prerequisites</span></span>
<span data-ttu-id="bcdb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcdb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcdb3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcdb3-111">Permission type</span></span>|<span data-ttu-id="bcdb3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcdb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcdb3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcdb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcdb3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdb3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bcdb3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcdb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcdb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-116">Not supported.</span></span>|
|<span data-ttu-id="bcdb3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcdb3-117">Application</span></span>|<span data-ttu-id="bcdb3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcdb3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcdb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bcdb3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcdb3-120">Request headers</span></span>
|<span data-ttu-id="bcdb3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcdb3-121">Header</span></span>|<span data-ttu-id="bcdb3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcdb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcdb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcdb3-123">Authorization</span></span>|<span data-ttu-id="bcdb3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bcdb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcdb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcdb3-125">Accept</span></span>|<span data-ttu-id="bcdb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcdb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcdb3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcdb3-127">Request body</span></span>
<span data-ttu-id="bcdb3-128">В тексте запроса укажите представление JSON для объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bcdb3-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="bcdb3-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="bcdb3-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="bcdb3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcdb3-130">Property</span></span>|<span data-ttu-id="bcdb3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bcdb3-131">Type</span></span>|<span data-ttu-id="bcdb3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bcdb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcdb3-133">id</span><span class="sxs-lookup"><span data-stu-id="bcdb3-133">id</span></span>|<span data-ttu-id="bcdb3-134">String</span><span class="sxs-lookup"><span data-stu-id="bcdb3-134">String</span></span>|<span data-ttu-id="bcdb3-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-135">UUID for the object</span></span>|
|<span data-ttu-id="bcdb3-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bcdb3-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="bcdb3-137">String</span><span class="sxs-lookup"><span data-stu-id="bcdb3-137">String</span></span>|<span data-ttu-id="bcdb3-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="bcdb3-139">userId</span><span class="sxs-lookup"><span data-stu-id="bcdb3-139">userId</span></span>|<span data-ttu-id="bcdb3-140">String</span><span class="sxs-lookup"><span data-stu-id="bcdb3-140">String</span></span>|<span data-ttu-id="bcdb3-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="bcdb3-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="bcdb3-142">mobileAppList</span></span>|<span data-ttu-id="bcdb3-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bcdb3-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="bcdb3-144">Список целей полезных данных и состояния для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="bcdb3-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcdb3-145">Response</span></span>
<span data-ttu-id="bcdb3-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcdb3-147">Пример</span><span class="sxs-lookup"><span data-stu-id="bcdb3-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcdb3-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcdb3-148">Request</span></span>
<span data-ttu-id="bcdb3-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 769

{
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

### <a name="response"></a><span data-ttu-id="bcdb3-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcdb3-150">Response</span></span>
<span data-ttu-id="bcdb3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bcdb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





