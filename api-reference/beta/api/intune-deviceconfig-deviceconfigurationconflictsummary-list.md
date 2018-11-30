---
title: Список deviceConfigurationConflictSummaries
description: Свойства списка и связей объектов deviceConfigurationConflictSummary.
ms.openlocfilehash: d1d81560eafb59c2915f3bae3388710ded99f74c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081420"
---
# <a name="list-deviceconfigurationconflictsummaries"></a><span data-ttu-id="b3275-103">Список deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="b3275-103">List deviceConfigurationConflictSummaries</span></span>

> <span data-ttu-id="b3275-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3275-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3275-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3275-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3275-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3275-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3275-107">Свойства списка и связей объектов [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b3275-107">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3275-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3275-108">Prerequisites</span></span>
<span data-ttu-id="b3275-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3275-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3275-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3275-111">Permission type</span></span>|<span data-ttu-id="b3275-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3275-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3275-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3275-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3275-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3275-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b3275-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3275-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3275-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3275-116">Not supported.</span></span>|
|<span data-ttu-id="b3275-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3275-117">Application</span></span>|<span data-ttu-id="b3275-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3275-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3275-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3275-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="b3275-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3275-120">Request headers</span></span>
|<span data-ttu-id="b3275-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3275-121">Header</span></span>|<span data-ttu-id="b3275-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3275-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3275-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3275-123">Authorization</span></span>|<span data-ttu-id="b3275-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b3275-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3275-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3275-125">Accept</span></span>|<span data-ttu-id="b3275-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3275-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3275-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3275-127">Request body</span></span>
<span data-ttu-id="b3275-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3275-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3275-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3275-129">Response</span></span>
<span data-ttu-id="b3275-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3275-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3275-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b3275-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3275-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3275-132">Request</span></span>
<span data-ttu-id="b3275-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3275-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### <a name="response"></a><span data-ttu-id="b3275-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3275-134">Response</span></span>
<span data-ttu-id="b3275-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b3275-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
      "conflictingDeviceConfigurations": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
      "contributingSettings": [
        "Contributing Settings value"
      ],
      "deviceCheckinsImpacted": 6
    }
  ]
}
```





