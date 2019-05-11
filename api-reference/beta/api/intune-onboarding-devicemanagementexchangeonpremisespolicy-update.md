---
title: Обновление Девицеманажементексчанжеонпремисесполици
description: Обновление свойств объекта Девицеманажементексчанжеонпремисесполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84813ed63976f298e2b768e96ea10b9f9cf6dec8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900112"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="ba64f-103">Обновление Девицеманажементексчанжеонпремисесполици</span><span class="sxs-lookup"><span data-stu-id="ba64f-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="ba64f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba64f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba64f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba64f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba64f-106">Обновление свойств объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ba64f-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba64f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba64f-107">Prerequisites</span></span>
<span data-ttu-id="ba64f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba64f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba64f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba64f-110">Permission type</span></span>|<span data-ttu-id="ba64f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba64f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba64f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba64f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba64f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba64f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba64f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba64f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba64f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba64f-115">Not supported.</span></span>|
|<span data-ttu-id="ba64f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba64f-116">Application</span></span>|<span data-ttu-id="ba64f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba64f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba64f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba64f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ba64f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba64f-119">Request headers</span></span>
|<span data-ttu-id="ba64f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba64f-120">Header</span></span>|<span data-ttu-id="ba64f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba64f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba64f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba64f-122">Authorization</span></span>|<span data-ttu-id="ba64f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba64f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba64f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba64f-124">Accept</span></span>|<span data-ttu-id="ba64f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba64f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba64f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba64f-126">Request body</span></span>
<span data-ttu-id="ba64f-127">В тексте запроса добавьте представление объекта [Девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba64f-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="ba64f-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ba64f-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="ba64f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba64f-129">Property</span></span>|<span data-ttu-id="ba64f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba64f-130">Type</span></span>|<span data-ttu-id="ba64f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba64f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba64f-132">id</span><span class="sxs-lookup"><span data-stu-id="ba64f-132">id</span></span>|<span data-ttu-id="ba64f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ba64f-133">String</span></span>|<span data-ttu-id="ba64f-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba64f-134">Not yet documented</span></span>|
|<span data-ttu-id="ba64f-135">Нотификатионконтент</span><span class="sxs-lookup"><span data-stu-id="ba64f-135">notificationContent</span></span>|<span data-ttu-id="ba64f-136">Binary</span><span class="sxs-lookup"><span data-stu-id="ba64f-136">Binary</span></span>|<span data-ttu-id="ba64f-137">Текст уведомления, который будет отправляться пользователям, помещенным в карантин этой политикой.</span><span class="sxs-lookup"><span data-stu-id="ba64f-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="ba64f-138">Это HTML-кодированный массив байтов в кодировке UTF8.</span><span class="sxs-lookup"><span data-stu-id="ba64f-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="ba64f-139">Дефаултакцесслевел</span><span class="sxs-lookup"><span data-stu-id="ba64f-139">defaultAccessLevel</span></span>|[<span data-ttu-id="ba64f-140">Девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="ba64f-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="ba64f-141">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba64f-141">Default access state in Exchange.</span></span> <span data-ttu-id="ba64f-142">Это правило применяется глобально ко всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba64f-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="ba64f-143">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="ba64f-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="ba64f-144">Акцессрулес</span><span class="sxs-lookup"><span data-stu-id="ba64f-144">accessRules</span></span>|<span data-ttu-id="ba64f-145">Коллекция [девицеманажементексчанжеакцессруле](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="ba64f-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="ba64f-146">Список правил доступа к устройствам в Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba64f-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="ba64f-147">Правила доступа применяются глобально ко всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="ba64f-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="ba64f-148">Кновндевицеклассес</span><span class="sxs-lookup"><span data-stu-id="ba64f-148">knownDeviceClasses</span></span>|<span data-ttu-id="ba64f-149">Коллекция [девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="ba64f-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="ba64f-150">Список классов устройств, известных для Exchange</span><span class="sxs-lookup"><span data-stu-id="ba64f-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="ba64f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba64f-151">Response</span></span>
<span data-ttu-id="ba64f-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba64f-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba64f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ba64f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba64f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba64f-154">Request</span></span>
<span data-ttu-id="ba64f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba64f-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba64f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba64f-156">Response</span></span>
<span data-ttu-id="ba64f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba64f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




