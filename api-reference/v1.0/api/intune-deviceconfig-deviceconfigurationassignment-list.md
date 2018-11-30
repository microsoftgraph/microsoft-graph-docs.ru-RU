---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
ms.openlocfilehash: 6d8407f17d5ef1cb5ac771fd86bd4365d9e92876
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027240"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="4e7be-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4e7be-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="4e7be-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e7be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e7be-105">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4e7be-105">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e7be-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e7be-106">Prerequisites</span></span>
<span data-ttu-id="4e7be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e7be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e7be-109">Permission type</span></span>|<span data-ttu-id="4e7be-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e7be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e7be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e7be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e7be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e7be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e7be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e7be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7be-114">Not supported.</span></span>|
|<span data-ttu-id="4e7be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e7be-115">Application</span></span>|<span data-ttu-id="4e7be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e7be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e7be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4e7be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e7be-118">Request headers</span></span>
|<span data-ttu-id="4e7be-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e7be-119">Header</span></span>|<span data-ttu-id="4e7be-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4e7be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e7be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7be-121">Authorization</span></span>|<span data-ttu-id="4e7be-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e7be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e7be-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4e7be-123">Accept</span></span>|<span data-ttu-id="4e7be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7be-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e7be-125">Request body</span></span>
<span data-ttu-id="4e7be-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e7be-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7be-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e7be-127">Response</span></span>
<span data-ttu-id="4e7be-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7be-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e7be-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4e7be-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e7be-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e7be-130">Request</span></span>
<span data-ttu-id="4e7be-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e7be-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="4e7be-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e7be-132">Response</span></span>
<span data-ttu-id="4e7be-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4e7be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



