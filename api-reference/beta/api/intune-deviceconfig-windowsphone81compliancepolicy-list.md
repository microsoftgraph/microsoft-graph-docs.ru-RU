---
title: Перечисление объектов windowsPhone81CompliancePolicy
description: Список свойств и связей объектов windowsPhone81CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: c7ce1588e9be2258f81b89c961b5eb67cb499ee6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361553"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="f0a74-103">Перечисление объектов windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f0a74-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="f0a74-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0a74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0a74-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0a74-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0a74-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0a74-107">Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0a74-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0a74-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0a74-108">Prerequisites</span></span>
<span data-ttu-id="f0a74-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a74-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0a74-111">Permission type</span></span>|<span data-ttu-id="f0a74-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0a74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0a74-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0a74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0a74-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0a74-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f0a74-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0a74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0a74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a74-116">Not supported.</span></span>|
|<span data-ttu-id="f0a74-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0a74-117">Application</span></span>|<span data-ttu-id="f0a74-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a74-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0a74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0a74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f0a74-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0a74-120">Request headers</span></span>
|<span data-ttu-id="f0a74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0a74-121">Header</span></span>|<span data-ttu-id="f0a74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0a74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0a74-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0a74-123">Authorization</span></span>|<span data-ttu-id="f0a74-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0a74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0a74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0a74-125">Accept</span></span>|<span data-ttu-id="f0a74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0a74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a74-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0a74-127">Request body</span></span>
<span data-ttu-id="f0a74-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0a74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0a74-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0a74-129">Response</span></span>
<span data-ttu-id="f0a74-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0a74-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a74-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f0a74-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0a74-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0a74-132">Request</span></span>
<span data-ttu-id="f0a74-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0a74-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="f0a74-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0a74-134">Response</span></span>
<span data-ttu-id="f0a74-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0a74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```





