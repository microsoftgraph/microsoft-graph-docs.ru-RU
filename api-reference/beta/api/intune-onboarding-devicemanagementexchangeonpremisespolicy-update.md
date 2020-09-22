---
title: Обновление Девицеманажементексчанжеонпремисесполици
description: Обновление свойств объекта Девицеманажементексчанжеонпремисесполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 733691e67d0002848e84f4f9e105068f98e2d914
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072188"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="976ea-103">Обновление Девицеманажементексчанжеонпремисесполици</span><span class="sxs-lookup"><span data-stu-id="976ea-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="976ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="976ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="976ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="976ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="976ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="976ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="976ea-107">Обновление свойств объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="976ea-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="976ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="976ea-108">Prerequisites</span></span>
<span data-ttu-id="976ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="976ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="976ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="976ea-111">Permission type</span></span>|<span data-ttu-id="976ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="976ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="976ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="976ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="976ea-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="976ea-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="976ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="976ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="976ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="976ea-116">Not supported.</span></span>|
|<span data-ttu-id="976ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="976ea-117">Application</span></span>|<span data-ttu-id="976ea-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="976ea-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="976ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="976ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="976ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="976ea-120">Request headers</span></span>
|<span data-ttu-id="976ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="976ea-121">Header</span></span>|<span data-ttu-id="976ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="976ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="976ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="976ea-123">Authorization</span></span>|<span data-ttu-id="976ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="976ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="976ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="976ea-125">Accept</span></span>|<span data-ttu-id="976ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="976ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="976ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="976ea-127">Request body</span></span>
<span data-ttu-id="976ea-128">В тексте запроса добавьте представление объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="976ea-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="976ea-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="976ea-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="976ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="976ea-130">Property</span></span>|<span data-ttu-id="976ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="976ea-131">Type</span></span>|<span data-ttu-id="976ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="976ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="976ea-133">id</span><span class="sxs-lookup"><span data-stu-id="976ea-133">id</span></span>|<span data-ttu-id="976ea-134">String</span><span class="sxs-lookup"><span data-stu-id="976ea-134">String</span></span>|<span data-ttu-id="976ea-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="976ea-135">Not yet documented</span></span>|
|<span data-ttu-id="976ea-136">нотификатионконтент</span><span class="sxs-lookup"><span data-stu-id="976ea-136">notificationContent</span></span>|<span data-ttu-id="976ea-137">Binary</span><span class="sxs-lookup"><span data-stu-id="976ea-137">Binary</span></span>|<span data-ttu-id="976ea-138">Текст уведомления, который будет отправляться пользователям, помещенным в карантин этой политикой.</span><span class="sxs-lookup"><span data-stu-id="976ea-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="976ea-139">Это HTML-кодированный массив байтов в кодировке UTF8.</span><span class="sxs-lookup"><span data-stu-id="976ea-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="976ea-140">дефаултакцесслевел</span><span class="sxs-lookup"><span data-stu-id="976ea-140">defaultAccessLevel</span></span>|[<span data-ttu-id="976ea-141">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="976ea-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="976ea-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="976ea-142">Default access state in Exchange.</span></span> <span data-ttu-id="976ea-143">Это правило применяется глобально ко всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="976ea-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="976ea-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="976ea-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="976ea-145">акцессрулес</span><span class="sxs-lookup"><span data-stu-id="976ea-145">accessRules</span></span>|<span data-ttu-id="976ea-146">Коллекция [девицеманажементексчанжеакцессруле](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="976ea-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="976ea-147">Список правил доступа к устройствам в Exchange.</span><span class="sxs-lookup"><span data-stu-id="976ea-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="976ea-148">Правила доступа применяются глобально ко всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="976ea-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="976ea-149">кновндевицеклассес</span><span class="sxs-lookup"><span data-stu-id="976ea-149">knownDeviceClasses</span></span>|<span data-ttu-id="976ea-150">Коллекция [девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="976ea-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="976ea-151">Список классов устройств, известных для Exchange</span><span class="sxs-lookup"><span data-stu-id="976ea-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="976ea-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="976ea-152">Response</span></span>
<span data-ttu-id="976ea-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="976ea-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="976ea-154">Пример</span><span class="sxs-lookup"><span data-stu-id="976ea-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="976ea-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="976ea-155">Request</span></span>
<span data-ttu-id="976ea-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="976ea-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="976ea-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="976ea-157">Response</span></span>
<span data-ttu-id="976ea-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="976ea-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```






