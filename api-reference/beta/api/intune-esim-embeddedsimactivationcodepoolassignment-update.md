---
title: Обновление встроенныхSIMActivationCodePoolAssignment
description: Обновление свойств встроенного объектаSIMActivationCodePoolAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1fbed18e4b41df0e52e52d50fd73fe89aaf2bda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126082"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="e1768-103">Обновление встроенныхSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e1768-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="e1768-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1768-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1768-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1768-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1768-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1768-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1768-107">Обновление свойств встроенного [объектаSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e1768-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1768-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1768-108">Prerequisites</span></span>
<span data-ttu-id="e1768-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1768-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1768-111">Permission type</span></span>|<span data-ttu-id="e1768-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1768-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1768-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1768-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1768-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1768-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1768-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1768-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1768-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1768-116">Not supported.</span></span>|
|<span data-ttu-id="e1768-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e1768-117">Application</span></span>|<span data-ttu-id="e1768-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1768-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1768-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1768-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e1768-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1768-120">Request headers</span></span>
|<span data-ttu-id="e1768-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1768-121">Header</span></span>|<span data-ttu-id="e1768-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1768-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1768-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1768-123">Authorization</span></span>|<span data-ttu-id="e1768-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1768-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1768-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1768-125">Accept</span></span>|<span data-ttu-id="e1768-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1768-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1768-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1768-127">Request body</span></span>
<span data-ttu-id="e1768-128">В теле запроса поставляем представление JSON для встроенного [объектаSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e1768-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="e1768-129">В следующей таблице показаны свойства, необходимые при создании [встроенногоSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e1768-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="e1768-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1768-130">Property</span></span>|<span data-ttu-id="e1768-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1768-131">Type</span></span>|<span data-ttu-id="e1768-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1768-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1768-133">id</span><span class="sxs-lookup"><span data-stu-id="e1768-133">id</span></span>|<span data-ttu-id="e1768-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e1768-134">String</span></span>|<span data-ttu-id="e1768-135">Уникальный идентификатор для встроенного пула активации SIM-кода.</span><span class="sxs-lookup"><span data-stu-id="e1768-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="e1768-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="e1768-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e1768-137">target</span><span class="sxs-lookup"><span data-stu-id="e1768-137">target</span></span>|[<span data-ttu-id="e1768-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e1768-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e1768-139">Тип групп, целевых для встроенного пула кодов активации SIM.</span><span class="sxs-lookup"><span data-stu-id="e1768-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="e1768-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1768-140">Response</span></span>
<span data-ttu-id="e1768-141">В случае успешного выполнения этот метод возвращает код отклика и обновленный встроенный `200 OK` [объектSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e1768-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1768-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e1768-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1768-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1768-143">Request</span></span>
<span data-ttu-id="e1768-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1768-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="e1768-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1768-145">Response</span></span>
<span data-ttu-id="e1768-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1768-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




