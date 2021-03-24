---
title: Обновление deviceManagementSettingCategory
description: Обновление свойств объекта deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b98199e9e5f691cbceead1b22657bb31c2fb6b6c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136638"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="92df5-103">Обновление deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="92df5-103">Update deviceManagementSettingCategory</span></span>

<span data-ttu-id="92df5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92df5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92df5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92df5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92df5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92df5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92df5-107">Обновление свойств объекта [deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="92df5-107">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92df5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92df5-108">Prerequisites</span></span>
<span data-ttu-id="92df5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92df5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92df5-111">Permission type</span></span>|<span data-ttu-id="92df5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92df5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92df5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92df5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92df5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92df5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92df5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92df5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92df5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92df5-116">Not supported.</span></span>|
|<span data-ttu-id="92df5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="92df5-117">Application</span></span>|<span data-ttu-id="92df5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92df5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92df5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92df5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="92df5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92df5-120">Request headers</span></span>
|<span data-ttu-id="92df5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92df5-121">Header</span></span>|<span data-ttu-id="92df5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92df5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92df5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92df5-123">Authorization</span></span>|<span data-ttu-id="92df5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92df5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92df5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92df5-125">Accept</span></span>|<span data-ttu-id="92df5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92df5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92df5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92df5-127">Request body</span></span>
<span data-ttu-id="92df5-128">В теле запроса поставляем представление JSON для [объекта deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="92df5-128">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="92df5-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="92df5-129">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="92df5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92df5-130">Property</span></span>|<span data-ttu-id="92df5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92df5-131">Type</span></span>|<span data-ttu-id="92df5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92df5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92df5-133">id</span><span class="sxs-lookup"><span data-stu-id="92df5-133">id</span></span>|<span data-ttu-id="92df5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="92df5-134">String</span></span>|<span data-ttu-id="92df5-135">ID категории</span><span class="sxs-lookup"><span data-stu-id="92df5-135">The category ID</span></span>|
|<span data-ttu-id="92df5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92df5-136">displayName</span></span>|<span data-ttu-id="92df5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="92df5-137">String</span></span>|<span data-ttu-id="92df5-138">Имя категории</span><span class="sxs-lookup"><span data-stu-id="92df5-138">The category name</span></span>|
|<span data-ttu-id="92df5-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="92df5-139">hasRequiredSetting</span></span>|<span data-ttu-id="92df5-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="92df5-140">Boolean</span></span>|<span data-ttu-id="92df5-141">Категория содержит требуемую настройку верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="92df5-141">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="92df5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="92df5-142">Response</span></span>
<span data-ttu-id="92df5-143">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="92df5-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92df5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="92df5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="92df5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="92df5-145">Request</span></span>
<span data-ttu-id="92df5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92df5-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="92df5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="92df5-147">Response</span></span>
<span data-ttu-id="92df5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92df5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




