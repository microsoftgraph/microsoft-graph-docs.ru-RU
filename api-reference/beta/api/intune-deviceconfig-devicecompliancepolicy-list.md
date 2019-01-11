---
title: Перечисление объектов deviceCompliancePolicy
description: Список свойств и связей объектов deviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74f14e69ab4146f82b15476ccacb62e6ee0111fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891114"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="78c44-103">Перечисление объектов deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="78c44-103">List deviceCompliancePolicies</span></span>

> <span data-ttu-id="78c44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78c44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78c44-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78c44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c44-107">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="78c44-107">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78c44-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="78c44-108">Prerequisites</span></span>
<span data-ttu-id="78c44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78c44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78c44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78c44-111">Permission type</span></span>|<span data-ttu-id="78c44-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78c44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78c44-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78c44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78c44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78c44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78c44-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78c44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78c44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c44-116">Not supported.</span></span>|
|<span data-ttu-id="78c44-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78c44-117">Application</span></span>|<span data-ttu-id="78c44-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78c44-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78c44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="78c44-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78c44-120">Request headers</span></span>
|<span data-ttu-id="78c44-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78c44-121">Header</span></span>|<span data-ttu-id="78c44-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78c44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78c44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78c44-123">Authorization</span></span>|<span data-ttu-id="78c44-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="78c44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78c44-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78c44-125">Accept</span></span>|<span data-ttu-id="78c44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78c44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78c44-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78c44-127">Request body</span></span>
<span data-ttu-id="78c44-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78c44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78c44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="78c44-129">Response</span></span>
<span data-ttu-id="78c44-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78c44-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78c44-131">Пример</span><span class="sxs-lookup"><span data-stu-id="78c44-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="78c44-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="78c44-132">Request</span></span>
<span data-ttu-id="78c44-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78c44-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="78c44-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="78c44-134">Response</span></span>
<span data-ttu-id="78c44-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="78c44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```





