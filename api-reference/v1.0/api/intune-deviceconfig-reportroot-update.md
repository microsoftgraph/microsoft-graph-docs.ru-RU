---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef3ebef270c79af26a663c88cdc4857d5fb175fb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760764"
---
# <a name="update-reportroot"></a><span data-ttu-id="262b0-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="262b0-103">Update reportRoot</span></span>

<span data-ttu-id="262b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="262b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="262b0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="262b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="262b0-106">Обновление свойств объекта [reportRoot](../resources/intune-deviceconfig-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="262b0-106">Update the properties of a [reportRoot](../resources/intune-deviceconfig-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="262b0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="262b0-107">Prerequisites</span></span>
<span data-ttu-id="262b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="262b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="262b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="262b0-110">Permission type</span></span>|<span data-ttu-id="262b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="262b0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="262b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="262b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="262b0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262b0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="262b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="262b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="262b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="262b0-115">Not supported.</span></span>|
|<span data-ttu-id="262b0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="262b0-116">Application</span></span>|<span data-ttu-id="262b0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262b0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="262b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="262b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="262b0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="262b0-119">Request headers</span></span>
|<span data-ttu-id="262b0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="262b0-120">Header</span></span>|<span data-ttu-id="262b0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="262b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="262b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="262b0-122">Authorization</span></span>|<span data-ttu-id="262b0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="262b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="262b0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="262b0-124">Accept</span></span>|<span data-ttu-id="262b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="262b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="262b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="262b0-126">Request body</span></span>
<span data-ttu-id="262b0-127">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-deviceconfig-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="262b0-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-deviceconfig-reportroot.md) object.</span></span>

<span data-ttu-id="262b0-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-deviceconfig-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="262b0-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-deviceconfig-reportroot.md).</span></span>

|<span data-ttu-id="262b0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="262b0-129">Property</span></span>|<span data-ttu-id="262b0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="262b0-130">Type</span></span>|<span data-ttu-id="262b0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="262b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="262b0-132">id</span><span class="sxs-lookup"><span data-stu-id="262b0-132">id</span></span>|<span data-ttu-id="262b0-133">String</span><span class="sxs-lookup"><span data-stu-id="262b0-133">String</span></span>|<span data-ttu-id="262b0-134">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="262b0-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="262b0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="262b0-135">Response</span></span>
<span data-ttu-id="262b0-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-deviceconfig-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="262b0-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-deviceconfig-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="262b0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="262b0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="262b0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="262b0-138">Request</span></span>
<span data-ttu-id="262b0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="262b0-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 52

{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```

### <a name="response"></a><span data-ttu-id="262b0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="262b0-140">Response</span></span>
<span data-ttu-id="262b0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="262b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```




