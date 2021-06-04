---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d67e334b0f9ff3329bfa3bdfbd5436527461d9f
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732902"
---
# <a name="update-reportroot"></a><span data-ttu-id="bb464-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="bb464-103">Update reportRoot</span></span>

<span data-ttu-id="bb464-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb464-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb464-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb464-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb464-106">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="bb464-106">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb464-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb464-107">Prerequisites</span></span>
<span data-ttu-id="bb464-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb464-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb464-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb464-110">Permission type</span></span>|<span data-ttu-id="bb464-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb464-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb464-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb464-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bb464-113">&nbsp;&nbsp;Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="bb464-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="bb464-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb464-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="bb464-115">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="bb464-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="bb464-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb464-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb464-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb464-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb464-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb464-118">Not supported.</span></span>|
|<span data-ttu-id="bb464-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb464-119">Application</span></span>|<span data-ttu-id="bb464-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb464-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb464-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb464-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="bb464-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb464-122">Request headers</span></span>
|<span data-ttu-id="bb464-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb464-123">Header</span></span>|<span data-ttu-id="bb464-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bb464-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb464-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb464-125">Authorization</span></span>|<span data-ttu-id="bb464-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb464-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb464-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bb464-127">Accept</span></span>|<span data-ttu-id="bb464-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bb464-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb464-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb464-129">Request body</span></span>
<span data-ttu-id="bb464-130">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb464-130">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="bb464-131">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="bb464-131">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="bb464-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb464-132">Property</span></span>|<span data-ttu-id="bb464-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bb464-133">Type</span></span>|<span data-ttu-id="bb464-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bb464-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb464-135">id</span><span class="sxs-lookup"><span data-stu-id="bb464-135">id</span></span>|<span data-ttu-id="bb464-136">String</span><span class="sxs-lookup"><span data-stu-id="bb464-136">String</span></span>|<span data-ttu-id="bb464-137">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="bb464-137">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="bb464-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb464-138">Response</span></span>
<span data-ttu-id="bb464-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb464-139">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb464-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bb464-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb464-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb464-141">Request</span></span>
<span data-ttu-id="bb464-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb464-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="bb464-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb464-143">Response</span></span>
<span data-ttu-id="bb464-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb464-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```














