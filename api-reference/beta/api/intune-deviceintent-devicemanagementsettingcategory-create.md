---
title: Создание Девицеманажементсеттингкатегори
description: Создание нового объекта Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7868d155dfd5fb5c0e18c2d3d224c708bddfe3b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986737"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="c96ce-103">Создание Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="c96ce-103">Create deviceManagementSettingCategory</span></span>

<span data-ttu-id="c96ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c96ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c96ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c96ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c96ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c96ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c96ce-107">Создание нового объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c96ce-107">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c96ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c96ce-108">Prerequisites</span></span>
<span data-ttu-id="c96ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c96ce-111">Permission type</span></span>|<span data-ttu-id="c96ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c96ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c96ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c96ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c96ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c96ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c96ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c96ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c96ce-116">Not supported.</span></span>|
|<span data-ttu-id="c96ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c96ce-117">Application</span></span>|<span data-ttu-id="c96ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c96ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c96ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="c96ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c96ce-120">Request headers</span></span>
|<span data-ttu-id="c96ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c96ce-121">Header</span></span>|<span data-ttu-id="c96ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c96ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c96ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c96ce-123">Authorization</span></span>|<span data-ttu-id="c96ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c96ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c96ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c96ce-125">Accept</span></span>|<span data-ttu-id="c96ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c96ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c96ce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c96ce-127">Request body</span></span>
<span data-ttu-id="c96ce-128">В тексте запроса добавьте представление объекта Девицеманажементсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c96ce-128">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="c96ce-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="c96ce-129">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="c96ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c96ce-130">Property</span></span>|<span data-ttu-id="c96ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c96ce-131">Type</span></span>|<span data-ttu-id="c96ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c96ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c96ce-133">id</span><span class="sxs-lookup"><span data-stu-id="c96ce-133">id</span></span>|<span data-ttu-id="c96ce-134">String</span><span class="sxs-lookup"><span data-stu-id="c96ce-134">String</span></span>|<span data-ttu-id="c96ce-135">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="c96ce-135">The category ID</span></span>|
|<span data-ttu-id="c96ce-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c96ce-136">displayName</span></span>|<span data-ttu-id="c96ce-137">String</span><span class="sxs-lookup"><span data-stu-id="c96ce-137">String</span></span>|<span data-ttu-id="c96ce-138">Имя категории</span><span class="sxs-lookup"><span data-stu-id="c96ce-138">The category name</span></span>|
|<span data-ttu-id="c96ce-139">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="c96ce-139">hasRequiredSetting</span></span>|<span data-ttu-id="c96ce-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c96ce-140">Boolean</span></span>|<span data-ttu-id="c96ce-141">Категория содержит параметры, необходимые для верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="c96ce-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="c96ce-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c96ce-142">Response</span></span>
<span data-ttu-id="c96ce-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c96ce-143">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c96ce-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c96ce-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c96ce-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c96ce-145">Request</span></span>
<span data-ttu-id="c96ce-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c96ce-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="c96ce-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c96ce-147">Response</span></span>
<span data-ttu-id="c96ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c96ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```






