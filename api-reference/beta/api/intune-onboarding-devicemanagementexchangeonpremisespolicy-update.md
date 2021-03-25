---
title: Обновление deviceManagementExchangeOnPremisesPolicy
description: Обновление свойств объекта deviceManagementExchangeOnPremisesPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d1aaec016c95845c0f33ede2f413811a58fa44c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156893"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="e720e-103">Обновление deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="e720e-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="e720e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e720e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e720e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e720e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e720e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e720e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e720e-107">Обновление свойств объекта [deviceManagementExchangeOnPremisesPolicy.](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e720e-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e720e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e720e-108">Prerequisites</span></span>
<span data-ttu-id="e720e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e720e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e720e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e720e-111">Permission type</span></span>|<span data-ttu-id="e720e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e720e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e720e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e720e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e720e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e720e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e720e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e720e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e720e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e720e-116">Not supported.</span></span>|
|<span data-ttu-id="e720e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e720e-117">Application</span></span>|<span data-ttu-id="e720e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e720e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e720e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e720e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e720e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e720e-120">Request headers</span></span>
|<span data-ttu-id="e720e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e720e-121">Header</span></span>|<span data-ttu-id="e720e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e720e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e720e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e720e-123">Authorization</span></span>|<span data-ttu-id="e720e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e720e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e720e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e720e-125">Accept</span></span>|<span data-ttu-id="e720e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e720e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e720e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e720e-127">Request body</span></span>
<span data-ttu-id="e720e-128">В теле запроса поставляем представление JSON для [объекта deviceManagementExchangeOnPremisesPolicy.](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e720e-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="e720e-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementExchangeOnPremisesPolicy.](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e720e-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="e720e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e720e-130">Property</span></span>|<span data-ttu-id="e720e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e720e-131">Type</span></span>|<span data-ttu-id="e720e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e720e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e720e-133">id</span><span class="sxs-lookup"><span data-stu-id="e720e-133">id</span></span>|<span data-ttu-id="e720e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e720e-134">String</span></span>|<span data-ttu-id="e720e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e720e-135">Not yet documented</span></span>|
|<span data-ttu-id="e720e-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="e720e-136">notificationContent</span></span>|<span data-ttu-id="e720e-137">Binary</span><span class="sxs-lookup"><span data-stu-id="e720e-137">Binary</span></span>|<span data-ttu-id="e720e-138">Текст уведомления, который будет отправлен пользователям, на карантин по этой политике.</span><span class="sxs-lookup"><span data-stu-id="e720e-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="e720e-139">Это HTML массива UTF8 с кодом byte.</span><span class="sxs-lookup"><span data-stu-id="e720e-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="e720e-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e720e-140">defaultAccessLevel</span></span>|[<span data-ttu-id="e720e-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e720e-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="e720e-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e720e-142">Default access state in Exchange.</span></span> <span data-ttu-id="e720e-143">Это правило применяется глобально ко всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="e720e-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="e720e-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="e720e-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="e720e-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="e720e-145">accessRules</span></span>|<span data-ttu-id="e720e-146">[коллекция deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="e720e-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="e720e-147">Список правил доступа к устройствам в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e720e-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="e720e-148">Правила доступа глобально применяются ко всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="e720e-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="e720e-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="e720e-149">knownDeviceClasses</span></span>|<span data-ttu-id="e720e-150">[коллекция deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="e720e-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="e720e-151">Список классов устройств, известных Exchange</span><span class="sxs-lookup"><span data-stu-id="e720e-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="e720e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e720e-152">Response</span></span>
<span data-ttu-id="e720e-153">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e720e-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e720e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e720e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e720e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e720e-155">Request</span></span>
<span data-ttu-id="e720e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e720e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e720e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e720e-157">Response</span></span>
<span data-ttu-id="e720e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e720e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




