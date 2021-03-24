---
title: Обновление deviceManagementIntentSettingCategory
description: Обновление свойств объекта deviceManagementIntentSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d74309de7de867267a9cfc9abaaf31ff360175d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130919"
---
# <a name="update-devicemanagementintentsettingcategory"></a><span data-ttu-id="1d875-103">Обновление deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="1d875-103">Update deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="1d875-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d875-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d875-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d875-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d875-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d875-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d875-107">Обновление свойств объекта [deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-107">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d875-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d875-108">Prerequisites</span></span>
<span data-ttu-id="1d875-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d875-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d875-111">Permission type</span></span>|<span data-ttu-id="1d875-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d875-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d875-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d875-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d875-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d875-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d875-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d875-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d875-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d875-116">Not supported.</span></span>|
|<span data-ttu-id="1d875-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1d875-117">Application</span></span>|<span data-ttu-id="1d875-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d875-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d875-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d875-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="1d875-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d875-120">Request headers</span></span>
|<span data-ttu-id="1d875-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d875-121">Header</span></span>|<span data-ttu-id="1d875-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d875-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d875-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d875-123">Authorization</span></span>|<span data-ttu-id="1d875-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d875-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d875-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d875-125">Accept</span></span>|<span data-ttu-id="1d875-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d875-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d875-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d875-127">Request body</span></span>
<span data-ttu-id="1d875-128">В теле запроса поставляем представление JSON для [объекта deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-128">In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

<span data-ttu-id="1d875-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-129">The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

|<span data-ttu-id="1d875-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d875-130">Property</span></span>|<span data-ttu-id="1d875-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d875-131">Type</span></span>|<span data-ttu-id="1d875-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d875-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d875-133">id</span><span class="sxs-lookup"><span data-stu-id="1d875-133">id</span></span>|<span data-ttu-id="1d875-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1d875-134">String</span></span>|<span data-ttu-id="1d875-135">ID категории, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="1d875-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1d875-136">displayName</span></span>|<span data-ttu-id="1d875-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1d875-137">String</span></span>|<span data-ttu-id="1d875-138">Имя категории, унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="1d875-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="1d875-139">hasRequiredSetting</span></span>|<span data-ttu-id="1d875-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d875-140">Boolean</span></span>|<span data-ttu-id="1d875-141">Категория содержит обязательный параметр верхнего уровня, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d875-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1d875-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d875-142">Response</span></span>
<span data-ttu-id="1d875-143">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1d875-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d875-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1d875-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d875-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d875-145">Request</span></span>
<span data-ttu-id="1d875-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d875-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="1d875-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d875-147">Response</span></span>
<span data-ttu-id="1d875-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d875-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




