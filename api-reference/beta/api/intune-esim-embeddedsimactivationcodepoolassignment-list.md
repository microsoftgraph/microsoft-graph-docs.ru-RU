---
title: Список Ембеддедсимактиватионкодепулассигнментс
description: Список свойств и связей объектов Ембеддедсимактиватионкодепулассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ee944e2804462261b359e36e4f9fb2010b933cb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792010"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="89d68-103">Список Ембеддедсимактиватионкодепулассигнментс</span><span class="sxs-lookup"><span data-stu-id="89d68-103">List embeddedSIMActivationCodePoolAssignments</span></span>

<span data-ttu-id="89d68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89d68-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89d68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d68-107">Список свойств и связей объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="89d68-107">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89d68-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89d68-108">Prerequisites</span></span>
<span data-ttu-id="89d68-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="89d68-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="89d68-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89d68-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89d68-111">Permission type</span></span>|<span data-ttu-id="89d68-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89d68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89d68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89d68-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d68-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89d68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89d68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d68-116">Not supported.</span></span>|
|<span data-ttu-id="89d68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89d68-117">Application</span></span>|<span data-ttu-id="89d68-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d68-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89d68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="89d68-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89d68-120">Request headers</span></span>
|<span data-ttu-id="89d68-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89d68-121">Header</span></span>|<span data-ttu-id="89d68-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89d68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d68-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89d68-123">Authorization</span></span>|<span data-ttu-id="89d68-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89d68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d68-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89d68-125">Accept</span></span>|<span data-ttu-id="89d68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89d68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d68-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89d68-127">Request body</span></span>
<span data-ttu-id="89d68-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89d68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89d68-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89d68-129">Response</span></span>
<span data-ttu-id="89d68-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89d68-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d68-131">Пример</span><span class="sxs-lookup"><span data-stu-id="89d68-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="89d68-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89d68-132">Request</span></span>
<span data-ttu-id="89d68-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89d68-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="89d68-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="89d68-134">Response</span></span>
<span data-ttu-id="89d68-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="89d68-135">Here is an example of the response.</span></span> <span data-ttu-id="89d68-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="89d68-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="89d68-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="89d68-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



