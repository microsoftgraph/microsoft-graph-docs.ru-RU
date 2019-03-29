---
title: Перечисление объектов managedAppOperation
description: Список свойств и связей объектов managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3ae31a7077b5003cf6c88f15afc4d45d9dda9a5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963060"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="e8732-103">Перечисление объектов managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e8732-103">List managedAppOperations</span></span>

> <span data-ttu-id="e8732-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8732-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8732-105">Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8732-105">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8732-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8732-106">Prerequisites</span></span>
<span data-ttu-id="e8732-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8732-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8732-109">Permission type</span></span>|<span data-ttu-id="e8732-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8732-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8732-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8732-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8732-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8732-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8732-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8732-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8732-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8732-114">Not supported.</span></span>|
|<span data-ttu-id="e8732-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8732-115">Application</span></span>|<span data-ttu-id="e8732-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8732-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8732-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8732-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="e8732-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8732-118">Request headers</span></span>
|<span data-ttu-id="e8732-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8732-119">Header</span></span>|<span data-ttu-id="e8732-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e8732-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8732-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8732-121">Authorization</span></span>|<span data-ttu-id="e8732-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8732-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8732-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e8732-123">Accept</span></span>|<span data-ttu-id="e8732-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e8732-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8732-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8732-125">Request body</span></span>
<span data-ttu-id="e8732-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8732-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8732-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8732-127">Response</span></span>
<span data-ttu-id="e8732-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e8732-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8732-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e8732-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8732-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8732-130">Request</span></span>
<span data-ttu-id="e8732-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8732-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="e8732-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8732-132">Response</span></span>
<span data-ttu-id="e8732-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8732-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```



