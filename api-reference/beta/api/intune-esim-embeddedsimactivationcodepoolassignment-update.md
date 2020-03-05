---
title: Обновление Ембеддедсимактиватионкодепулассигнмент
description: Обновление свойств объекта Ембеддедсимактиватионкодепулассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45f951f7de2c21843354dfe58e213bbe3ebabcd1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466033"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="d4b7f-103">Обновление Ембеддедсимактиватионкодепулассигнмент</span><span class="sxs-lookup"><span data-stu-id="d4b7f-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="d4b7f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4b7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4b7f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4b7f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4b7f-107">Обновление свойств объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b7f-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4b7f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4b7f-108">Prerequisites</span></span>
<span data-ttu-id="d4b7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4b7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b7f-111">Permission type</span></span>|<span data-ttu-id="d4b7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4b7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4b7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4b7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4b7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4b7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4b7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4b7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-116">Not supported.</span></span>|
|<span data-ttu-id="d4b7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4b7f-117">Application</span></span>|<span data-ttu-id="d4b7f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b7f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4b7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4b7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d4b7f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4b7f-120">Request headers</span></span>
|<span data-ttu-id="d4b7f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4b7f-121">Header</span></span>|<span data-ttu-id="d4b7f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4b7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4b7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4b7f-123">Authorization</span></span>|<span data-ttu-id="d4b7f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4b7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4b7f-125">Accept</span></span>|<span data-ttu-id="d4b7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4b7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b7f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4b7f-127">Request body</span></span>
<span data-ttu-id="d4b7f-128">В тексте запроса добавьте представление объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="d4b7f-129">В следующей таблице приведены свойства, необходимые при создании [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d4b7f-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="d4b7f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4b7f-130">Property</span></span>|<span data-ttu-id="d4b7f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4b7f-131">Type</span></span>|<span data-ttu-id="d4b7f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4b7f-133">id</span><span class="sxs-lookup"><span data-stu-id="d4b7f-133">id</span></span>|<span data-ttu-id="d4b7f-134">String</span><span class="sxs-lookup"><span data-stu-id="d4b7f-134">String</span></span>|<span data-ttu-id="d4b7f-135">Уникальный идентификатор для назначения внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="d4b7f-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d4b7f-137">target</span><span class="sxs-lookup"><span data-stu-id="d4b7f-137">target</span></span>|[<span data-ttu-id="d4b7f-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d4b7f-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d4b7f-139">Тип групп, на которые ссылается встроенный пул кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="d4b7f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b7f-140">Response</span></span>
<span data-ttu-id="d4b7f-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4b7f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d4b7f-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4b7f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4b7f-143">Request</span></span>
<span data-ttu-id="d4b7f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d4b7f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b7f-145">Response</span></span>
<span data-ttu-id="d4b7f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4b7f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





