---
title: Обновление mobileAppIntentAndState
description: Обновление свойства объекта mobileAppIntentAndState.
author: tfitzmac
ms.openlocfilehash: d219e6d9d146f71c4979973e7f6510010fe2fa92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303187"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="02438-103">Обновление mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="02438-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="02438-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02438-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02438-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02438-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02438-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02438-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02438-107">Обновление свойства объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="02438-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02438-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02438-108">Prerequisites</span></span>
<span data-ttu-id="02438-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02438-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02438-111">Permission type</span></span>|<span data-ttu-id="02438-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02438-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02438-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02438-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02438-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="02438-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02438-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02438-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02438-116">Not supported.</span></span>|
|<span data-ttu-id="02438-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02438-117">Application</span></span>|<span data-ttu-id="02438-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02438-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02438-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02438-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="02438-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02438-120">Request headers</span></span>
|<span data-ttu-id="02438-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02438-121">Header</span></span>|<span data-ttu-id="02438-122">Значение</span><span class="sxs-lookup"><span data-stu-id="02438-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02438-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02438-123">Authorization</span></span>|<span data-ttu-id="02438-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="02438-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02438-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02438-125">Accept</span></span>|<span data-ttu-id="02438-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02438-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02438-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02438-127">Request body</span></span>
<span data-ttu-id="02438-128">В тексте запроса укажите представление JSON для объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="02438-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="02438-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="02438-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="02438-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="02438-130">Property</span></span>|<span data-ttu-id="02438-131">Тип</span><span class="sxs-lookup"><span data-stu-id="02438-131">Type</span></span>|<span data-ttu-id="02438-132">Описание</span><span class="sxs-lookup"><span data-stu-id="02438-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02438-133">id</span><span class="sxs-lookup"><span data-stu-id="02438-133">id</span></span>|<span data-ttu-id="02438-134">String</span><span class="sxs-lookup"><span data-stu-id="02438-134">String</span></span>|<span data-ttu-id="02438-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="02438-135">UUID for the object</span></span>|
|<span data-ttu-id="02438-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="02438-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="02438-137">String</span><span class="sxs-lookup"><span data-stu-id="02438-137">String</span></span>|<span data-ttu-id="02438-138">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="02438-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="02438-139">userId</span><span class="sxs-lookup"><span data-stu-id="02438-139">userId</span></span>|<span data-ttu-id="02438-140">String</span><span class="sxs-lookup"><span data-stu-id="02438-140">String</span></span>|<span data-ttu-id="02438-141">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="02438-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="02438-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="02438-142">mobileAppList</span></span>|<span data-ttu-id="02438-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="02438-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="02438-144">Список целей полезных данных и состояния для клиента.</span><span class="sxs-lookup"><span data-stu-id="02438-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="02438-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="02438-145">Response</span></span>
<span data-ttu-id="02438-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02438-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02438-147">Пример</span><span class="sxs-lookup"><span data-stu-id="02438-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="02438-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="02438-148">Request</span></span>
<span data-ttu-id="02438-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02438-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02438-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="02438-150">Response</span></span>
<span data-ttu-id="02438-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="02438-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





