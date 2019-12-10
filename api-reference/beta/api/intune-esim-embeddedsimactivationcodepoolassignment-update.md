---
title: Обновление Ембеддедсимактиватионкодепулассигнмент
description: Обновление свойств объекта Ембеддедсимактиватионкодепулассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60c73bfa768489b5fd78de77ad513e4c9cc398f1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943560"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="f77d2-103">Обновление Ембеддедсимактиватионкодепулассигнмент</span><span class="sxs-lookup"><span data-stu-id="f77d2-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="f77d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f77d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f77d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77d2-106">Обновление свойств объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f77d2-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77d2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f77d2-107">Prerequisites</span></span>
<span data-ttu-id="f77d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f77d2-110">Permission type</span></span>|<span data-ttu-id="f77d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f77d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f77d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f77d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f77d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f77d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77d2-115">Not supported.</span></span>|
|<span data-ttu-id="f77d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f77d2-116">Application</span></span>|<span data-ttu-id="f77d2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77d2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f77d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f77d2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f77d2-119">Request headers</span></span>
|<span data-ttu-id="f77d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f77d2-120">Header</span></span>|<span data-ttu-id="f77d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f77d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f77d2-122">Authorization</span></span>|<span data-ttu-id="f77d2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f77d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77d2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f77d2-124">Accept</span></span>|<span data-ttu-id="f77d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f77d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77d2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f77d2-126">Request body</span></span>
<span data-ttu-id="f77d2-127">В тексте запроса добавьте представление объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f77d2-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="f77d2-128">В следующей таблице приведены свойства, необходимые при создании [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f77d2-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="f77d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f77d2-129">Property</span></span>|<span data-ttu-id="f77d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f77d2-130">Type</span></span>|<span data-ttu-id="f77d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f77d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77d2-132">id</span><span class="sxs-lookup"><span data-stu-id="f77d2-132">id</span></span>|<span data-ttu-id="f77d2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f77d2-133">String</span></span>|<span data-ttu-id="f77d2-134">Уникальный идентификатор для назначения внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77d2-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="f77d2-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="f77d2-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f77d2-136">target</span><span class="sxs-lookup"><span data-stu-id="f77d2-136">target</span></span>|[<span data-ttu-id="f77d2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f77d2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f77d2-138">Тип групп, на которые ссылается встроенный пул кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77d2-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="f77d2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f77d2-139">Response</span></span>
<span data-ttu-id="f77d2-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f77d2-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77d2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f77d2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77d2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f77d2-142">Request</span></span>
<span data-ttu-id="f77d2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f77d2-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f77d2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f77d2-144">Response</span></span>
<span data-ttu-id="f77d2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f77d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





