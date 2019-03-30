---
title: Перечисление объектов managedAppOperation
description: Список свойств и связей объектов managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fff514f3b98c119c9678489ed3cf593c9c6ca10
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964089"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="2336a-103">Перечисление объектов managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="2336a-103">List managedAppOperations</span></span>

> <span data-ttu-id="2336a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2336a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2336a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2336a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2336a-106">Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336a-106">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2336a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2336a-107">Prerequisites</span></span>
<span data-ttu-id="2336a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2336a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2336a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2336a-110">Permission type</span></span>|<span data-ttu-id="2336a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2336a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2336a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2336a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2336a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2336a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2336a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2336a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2336a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2336a-115">Not supported.</span></span>|
|<span data-ttu-id="2336a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2336a-116">Application</span></span>|<span data-ttu-id="2336a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2336a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2336a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2336a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="2336a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2336a-119">Request headers</span></span>
|<span data-ttu-id="2336a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2336a-120">Header</span></span>|<span data-ttu-id="2336a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2336a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2336a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2336a-122">Authorization</span></span>|<span data-ttu-id="2336a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2336a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2336a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2336a-124">Accept</span></span>|<span data-ttu-id="2336a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2336a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2336a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2336a-126">Request body</span></span>
<span data-ttu-id="2336a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2336a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2336a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2336a-128">Response</span></span>
<span data-ttu-id="2336a-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2336a-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2336a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2336a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2336a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2336a-131">Request</span></span>
<span data-ttu-id="2336a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2336a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="2336a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2336a-133">Response</span></span>
<span data-ttu-id="2336a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2336a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




