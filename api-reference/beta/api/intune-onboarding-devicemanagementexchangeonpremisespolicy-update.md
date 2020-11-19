---
title: Обновление Девицеманажементексчанжеонпремисесполици
description: Обновление свойств объекта Девицеманажементексчанжеонпремисесполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8ebb1b0eebd69461f6f9624be1e2b7588a74c2b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211644"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="22cf2-103">Обновление Девицеманажементексчанжеонпремисесполици</span><span class="sxs-lookup"><span data-stu-id="22cf2-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="22cf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22cf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22cf2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22cf2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22cf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22cf2-107">Обновление свойств объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="22cf2-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22cf2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22cf2-108">Prerequisites</span></span>
<span data-ttu-id="22cf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22cf2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22cf2-111">Permission type</span></span>|<span data-ttu-id="22cf2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22cf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22cf2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22cf2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22cf2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cf2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22cf2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22cf2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22cf2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cf2-116">Not supported.</span></span>|
|<span data-ttu-id="22cf2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="22cf2-117">Application</span></span>|<span data-ttu-id="22cf2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cf2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22cf2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22cf2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="22cf2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22cf2-120">Request headers</span></span>
|<span data-ttu-id="22cf2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22cf2-121">Header</span></span>|<span data-ttu-id="22cf2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22cf2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22cf2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22cf2-123">Authorization</span></span>|<span data-ttu-id="22cf2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22cf2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22cf2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22cf2-125">Accept</span></span>|<span data-ttu-id="22cf2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22cf2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22cf2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22cf2-127">Request body</span></span>
<span data-ttu-id="22cf2-128">В тексте запроса добавьте представление объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22cf2-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="22cf2-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="22cf2-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="22cf2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22cf2-130">Property</span></span>|<span data-ttu-id="22cf2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22cf2-131">Type</span></span>|<span data-ttu-id="22cf2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22cf2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22cf2-133">id</span><span class="sxs-lookup"><span data-stu-id="22cf2-133">id</span></span>|<span data-ttu-id="22cf2-134">String</span><span class="sxs-lookup"><span data-stu-id="22cf2-134">String</span></span>|<span data-ttu-id="22cf2-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="22cf2-135">Not yet documented</span></span>|
|<span data-ttu-id="22cf2-136">нотификатионконтент</span><span class="sxs-lookup"><span data-stu-id="22cf2-136">notificationContent</span></span>|<span data-ttu-id="22cf2-137">Binary</span><span class="sxs-lookup"><span data-stu-id="22cf2-137">Binary</span></span>|<span data-ttu-id="22cf2-138">Текст уведомления, который будет отправляться пользователям, помещенным в карантин этой политикой.</span><span class="sxs-lookup"><span data-stu-id="22cf2-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="22cf2-139">Это HTML-кодированный массив байтов в кодировке UTF8.</span><span class="sxs-lookup"><span data-stu-id="22cf2-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="22cf2-140">дефаултакцесслевел</span><span class="sxs-lookup"><span data-stu-id="22cf2-140">defaultAccessLevel</span></span>|[<span data-ttu-id="22cf2-141">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="22cf2-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="22cf2-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="22cf2-142">Default access state in Exchange.</span></span> <span data-ttu-id="22cf2-143">Это правило применяется глобально ко всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="22cf2-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="22cf2-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="22cf2-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="22cf2-145">акцессрулес</span><span class="sxs-lookup"><span data-stu-id="22cf2-145">accessRules</span></span>|<span data-ttu-id="22cf2-146">Коллекция [девицеманажементексчанжеакцессруле](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="22cf2-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="22cf2-147">Список правил доступа к устройствам в Exchange.</span><span class="sxs-lookup"><span data-stu-id="22cf2-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="22cf2-148">Правила доступа применяются глобально ко всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="22cf2-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="22cf2-149">кновндевицеклассес</span><span class="sxs-lookup"><span data-stu-id="22cf2-149">knownDeviceClasses</span></span>|<span data-ttu-id="22cf2-150">Коллекция [девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="22cf2-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="22cf2-151">Список классов устройств, известных для Exchange</span><span class="sxs-lookup"><span data-stu-id="22cf2-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="22cf2-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cf2-152">Response</span></span>
<span data-ttu-id="22cf2-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22cf2-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22cf2-154">Пример</span><span class="sxs-lookup"><span data-stu-id="22cf2-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="22cf2-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="22cf2-155">Request</span></span>
<span data-ttu-id="22cf2-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22cf2-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22cf2-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cf2-157">Response</span></span>
<span data-ttu-id="22cf2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22cf2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




