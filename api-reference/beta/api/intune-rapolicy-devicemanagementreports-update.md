---
title: Обновление Девицеманажементрепортс
description: Обновление свойств объекта Девицеманажементрепортс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f8160041f593972d28aaf8122a32c1d28360568
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302116"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="a4f8f-103">Обновление Девицеманажементрепортс</span><span class="sxs-lookup"><span data-stu-id="a4f8f-103">Update deviceManagementReports</span></span>

<span data-ttu-id="a4f8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4f8f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4f8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4f8f-107">Обновление свойств объекта [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="a4f8f-107">Update the properties of a [deviceManagementReports](../resources/intune-shared-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4f8f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4f8f-108">Prerequisites</span></span>
<span data-ttu-id="a4f8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f8f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f8f-111">Permission type</span></span>|<span data-ttu-id="a4f8f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4f8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4f8f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4f8f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f8f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4f8f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4f8f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-116">Not supported.</span></span>|
|<span data-ttu-id="a4f8f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4f8f-117">Application</span></span>|<span data-ttu-id="a4f8f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f8f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4f8f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="a4f8f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4f8f-120">Request headers</span></span>
|<span data-ttu-id="a4f8f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4f8f-121">Header</span></span>|<span data-ttu-id="a4f8f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4f8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4f8f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f8f-123">Authorization</span></span>|<span data-ttu-id="a4f8f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4f8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4f8f-125">Accept</span></span>|<span data-ttu-id="a4f8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4f8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f8f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4f8f-127">Request body</span></span>
<span data-ttu-id="a4f8f-128">В тексте запроса добавьте представление объекта [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-shared-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="a4f8f-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="a4f8f-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-shared-devicemanagementreports.md).</span></span>

|<span data-ttu-id="a4f8f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4f8f-130">Property</span></span>|<span data-ttu-id="a4f8f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f8f-131">Type</span></span>|<span data-ttu-id="a4f8f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4f8f-133">id</span><span class="sxs-lookup"><span data-stu-id="a4f8f-133">id</span></span>|<span data-ttu-id="a4f8f-134">String</span><span class="sxs-lookup"><span data-stu-id="a4f8f-134">String</span></span>|<span data-ttu-id="a4f8f-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="a4f8f-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="a4f8f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f8f-136">Response</span></span>
<span data-ttu-id="a4f8f-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементрепортс](../resources/intune-shared-devicemanagementreports.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-shared-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4f8f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a4f8f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4f8f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f8f-139">Request</span></span>
<span data-ttu-id="a4f8f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="a4f8f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f8f-141">Response</span></span>
<span data-ttu-id="a4f8f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4f8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




