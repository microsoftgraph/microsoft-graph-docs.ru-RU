---
title: Обновление deviceManagementReports
description: Обновление свойств объекта deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f887940b917225ee4def8b6def8cb8bf50c8854
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162001"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="2a366-103">Обновление deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="2a366-103">Update deviceManagementReports</span></span>

<span data-ttu-id="2a366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a366-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a366-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a366-107">Обновление свойств объекта [deviceManagementReports.](../resources/intune-rapolicy-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="2a366-107">Update the properties of a [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a366-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a366-108">Prerequisites</span></span>
<span data-ttu-id="2a366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a366-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a366-111">Permission type</span></span>|<span data-ttu-id="2a366-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a366-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a366-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a366-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a366-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a366-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a366-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a366-116">Not supported.</span></span>|
|<span data-ttu-id="2a366-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a366-117">Application</span></span>|<span data-ttu-id="2a366-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a366-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a366-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="2a366-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a366-120">Request headers</span></span>
|<span data-ttu-id="2a366-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a366-121">Header</span></span>|<span data-ttu-id="2a366-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2a366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a366-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a366-123">Authorization</span></span>|<span data-ttu-id="2a366-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a366-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a366-125">Accept</span></span>|<span data-ttu-id="2a366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a366-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a366-127">Request body</span></span>
<span data-ttu-id="2a366-128">В теле запроса укажу представление объекта [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="2a366-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="2a366-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementReports.](../resources/intune-rapolicy-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="2a366-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md).</span></span>

|<span data-ttu-id="2a366-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a366-130">Property</span></span>|<span data-ttu-id="2a366-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a366-131">Type</span></span>|<span data-ttu-id="2a366-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a366-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a366-133">id</span><span class="sxs-lookup"><span data-stu-id="2a366-133">id</span></span>|<span data-ttu-id="2a366-134">String</span><span class="sxs-lookup"><span data-stu-id="2a366-134">String</span></span>|<span data-ttu-id="2a366-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="2a366-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="2a366-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a366-136">Response</span></span>
<span data-ttu-id="2a366-137">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a366-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a366-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2a366-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a366-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a366-139">Request</span></span>
<span data-ttu-id="2a366-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a366-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="2a366-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a366-141">Response</span></span>
<span data-ttu-id="2a366-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a366-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




