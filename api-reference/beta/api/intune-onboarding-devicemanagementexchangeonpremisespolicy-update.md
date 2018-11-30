---
title: Обновление deviceManagementExchangeOnPremisesPolicy
description: Обновление свойства объекта deviceManagementExchangeOnPremisesPolicy.
ms.openlocfilehash: afc3df27d79b2cefab434126da8971f0fff5c8e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076008"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="7f9f5-103">Обновление deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="7f9f5-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="7f9f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f9f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f9f5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f9f5-107">Обновление свойства объекта [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7f9f5-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f9f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f9f5-108">Prerequisites</span></span>
<span data-ttu-id="7f9f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9f5-111">Permission type</span></span>|<span data-ttu-id="7f9f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f9f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f9f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f9f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f9f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f9f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f9f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f9f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f9f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-116">Not supported.</span></span>|
|<span data-ttu-id="7f9f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f9f5-117">Application</span></span>|<span data-ttu-id="7f9f5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f9f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f9f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7f9f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f9f5-120">Request headers</span></span>
|<span data-ttu-id="7f9f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f9f5-121">Header</span></span>|<span data-ttu-id="7f9f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f9f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f9f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f9f5-123">Authorization</span></span>|<span data-ttu-id="7f9f5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f9f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f9f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f9f5-125">Accept</span></span>|<span data-ttu-id="7f9f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f9f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f9f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f9f5-127">Request body</span></span>
<span data-ttu-id="7f9f5-128">В тексте запроса укажите представление JSON для объекта [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7f9f5-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="7f9f5-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f9f5-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="7f9f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f9f5-130">Property</span></span>|<span data-ttu-id="7f9f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f9f5-131">Type</span></span>|<span data-ttu-id="7f9f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f9f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f9f5-133">id</span><span class="sxs-lookup"><span data-stu-id="7f9f5-133">id</span></span>|<span data-ttu-id="7f9f5-134">String</span><span class="sxs-lookup"><span data-stu-id="7f9f5-134">String</span></span>|<span data-ttu-id="7f9f5-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7f9f5-135">Not yet documented</span></span>|
|<span data-ttu-id="7f9f5-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="7f9f5-136">notificationContent</span></span>|<span data-ttu-id="7f9f5-137">Двоичный</span><span class="sxs-lookup"><span data-stu-id="7f9f5-137">Binary</span></span>|<span data-ttu-id="7f9f5-138">Текст уведомления, которое будет отправляться пользователям в карантин для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="7f9f5-139">Это массив байтов кодировке UTF8 HTML.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="7f9f5-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="7f9f5-140">defaultAccessLevel</span></span>|[<span data-ttu-id="7f9f5-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="7f9f5-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="7f9f5-142">Состояние доступа по умолчанию в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-142">Default access state in Exchange.</span></span> <span data-ttu-id="7f9f5-143">Это правило применяется глобально во всей организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="7f9f5-144">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="7f9f5-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="7f9f5-145">accessRules</span></span>|<span data-ttu-id="7f9f5-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7f9f5-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="7f9f5-147">Список доступа устройств правила в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="7f9f5-148">Правила доступа к применяются глобально во всей организации Exchange</span><span class="sxs-lookup"><span data-stu-id="7f9f5-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="7f9f5-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="7f9f5-149">knownDeviceClasses</span></span>|<span data-ttu-id="7f9f5-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7f9f5-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="7f9f5-151">Список классов устройств в Exchange</span><span class="sxs-lookup"><span data-stu-id="7f9f5-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="7f9f5-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f9f5-152">Response</span></span>
<span data-ttu-id="7f9f5-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f9f5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7f9f5-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f9f5-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9f5-155">Request</span></span>
<span data-ttu-id="7f9f5-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9f5-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 586

{
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

### <a name="response"></a><span data-ttu-id="7f9f5-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f9f5-157">Response</span></span>
<span data-ttu-id="7f9f5-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7f9f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





