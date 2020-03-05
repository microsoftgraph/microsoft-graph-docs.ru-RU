---
title: Обновление Девицеманажементексчанжеонпремисесполици
description: Обновление свойств объекта Девицеманажементексчанжеонпремисесполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fdf7b8006e0181741956731da65024ca43571be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462126"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="3fa7a-103">Обновление Девицеманажементексчанжеонпремисесполици</span><span class="sxs-lookup"><span data-stu-id="3fa7a-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="3fa7a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3fa7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fa7a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fa7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fa7a-107">Обновление свойств объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3fa7a-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fa7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3fa7a-108">Prerequisites</span></span>
<span data-ttu-id="3fa7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa7a-111">Permission type</span></span>|<span data-ttu-id="3fa7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fa7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fa7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa7a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa7a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3fa7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-116">Not supported.</span></span>|
|<span data-ttu-id="3fa7a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fa7a-117">Application</span></span>|<span data-ttu-id="3fa7a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa7a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3fa7a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3fa7a-120">Request headers</span></span>
|<span data-ttu-id="3fa7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fa7a-121">Header</span></span>|<span data-ttu-id="3fa7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3fa7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fa7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa7a-123">Authorization</span></span>|<span data-ttu-id="3fa7a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fa7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fa7a-125">Accept</span></span>|<span data-ttu-id="3fa7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fa7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fa7a-127">Request body</span></span>
<span data-ttu-id="3fa7a-128">В тексте запроса добавьте представление объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="3fa7a-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3fa7a-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="3fa7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fa7a-130">Property</span></span>|<span data-ttu-id="3fa7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3fa7a-131">Type</span></span>|<span data-ttu-id="3fa7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fa7a-133">id</span><span class="sxs-lookup"><span data-stu-id="3fa7a-133">id</span></span>|<span data-ttu-id="3fa7a-134">String</span><span class="sxs-lookup"><span data-stu-id="3fa7a-134">String</span></span>|<span data-ttu-id="3fa7a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-135">Not yet documented</span></span>|
|<span data-ttu-id="3fa7a-136">нотификатионконтент</span><span class="sxs-lookup"><span data-stu-id="3fa7a-136">notificationContent</span></span>|<span data-ttu-id="3fa7a-137">Binary</span><span class="sxs-lookup"><span data-stu-id="3fa7a-137">Binary</span></span>|<span data-ttu-id="3fa7a-138">Текст уведомления, который будет отправляться пользователям, помещенным в карантин этой политикой.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="3fa7a-139">Это HTML-кодированный массив байтов в кодировке UTF8.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="3fa7a-140">дефаултакцесслевел</span><span class="sxs-lookup"><span data-stu-id="3fa7a-140">defaultAccessLevel</span></span>|[<span data-ttu-id="3fa7a-141">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="3fa7a-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="3fa7a-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-142">Default access state in Exchange.</span></span> <span data-ttu-id="3fa7a-143">Это правило применяется глобально ко всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="3fa7a-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="3fa7a-145">акцессрулес</span><span class="sxs-lookup"><span data-stu-id="3fa7a-145">accessRules</span></span>|<span data-ttu-id="3fa7a-146">Коллекция [девицеманажементексчанжеакцессруле](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="3fa7a-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="3fa7a-147">Список правил доступа к устройствам в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="3fa7a-148">Правила доступа применяются глобально ко всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="3fa7a-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="3fa7a-149">кновндевицеклассес</span><span class="sxs-lookup"><span data-stu-id="3fa7a-149">knownDeviceClasses</span></span>|<span data-ttu-id="3fa7a-150">Коллекция [девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="3fa7a-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="3fa7a-151">Список классов устройств, известных для Exchange</span><span class="sxs-lookup"><span data-stu-id="3fa7a-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="3fa7a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa7a-152">Response</span></span>
<span data-ttu-id="3fa7a-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa7a-154">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa7a-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa7a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa7a-155">Request</span></span>
<span data-ttu-id="3fa7a-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fa7a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa7a-157">Response</span></span>
<span data-ttu-id="3fa7a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fa7a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





