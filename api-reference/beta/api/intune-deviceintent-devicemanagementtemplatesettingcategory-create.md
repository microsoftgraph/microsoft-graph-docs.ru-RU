---
title: Создание deviceManagementTemplateSettingCategory
description: Создайте новый объект deviceManagementTemplateSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b616d74bdcbeee0179c8fa920a487bba69172d2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130856"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="76ce4-103">Создание deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="76ce4-103">Create deviceManagementTemplateSettingCategory</span></span>

<span data-ttu-id="76ce4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76ce4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76ce4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ce4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76ce4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76ce4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76ce4-107">Создайте новый [объект deviceManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76ce4-107">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76ce4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="76ce4-108">Prerequisites</span></span>
<span data-ttu-id="76ce4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76ce4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76ce4-111">Permission type</span></span>|<span data-ttu-id="76ce4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76ce4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76ce4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76ce4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76ce4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76ce4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76ce4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76ce4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76ce4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ce4-116">Not supported.</span></span>|
|<span data-ttu-id="76ce4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="76ce4-117">Application</span></span>|<span data-ttu-id="76ce4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76ce4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76ce4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76ce4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="76ce4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76ce4-120">Request headers</span></span>
|<span data-ttu-id="76ce4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76ce4-121">Header</span></span>|<span data-ttu-id="76ce4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76ce4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76ce4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76ce4-123">Authorization</span></span>|<span data-ttu-id="76ce4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76ce4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76ce4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76ce4-125">Accept</span></span>|<span data-ttu-id="76ce4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76ce4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76ce4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76ce4-127">Request body</span></span>
<span data-ttu-id="76ce4-128">В теле запроса поставляем представление JSON для объекта deviceManagementTemplateSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="76ce4-128">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="76ce4-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementTemplateSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="76ce4-129">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="76ce4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76ce4-130">Property</span></span>|<span data-ttu-id="76ce4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76ce4-131">Type</span></span>|<span data-ttu-id="76ce4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76ce4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76ce4-133">id</span><span class="sxs-lookup"><span data-stu-id="76ce4-133">id</span></span>|<span data-ttu-id="76ce4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="76ce4-134">String</span></span>|<span data-ttu-id="76ce4-135">ID категории, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76ce4-135">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="76ce4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="76ce4-136">displayName</span></span>|<span data-ttu-id="76ce4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="76ce4-137">String</span></span>|<span data-ttu-id="76ce4-138">Имя категории, унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76ce4-138">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="76ce4-139">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="76ce4-139">hasRequiredSetting</span></span>|<span data-ttu-id="76ce4-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="76ce4-140">Boolean</span></span>|<span data-ttu-id="76ce4-141">Категория содержит обязательный параметр верхнего уровня, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76ce4-141">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="76ce4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="76ce4-142">Response</span></span>
<span data-ttu-id="76ce4-143">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="76ce4-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76ce4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="76ce4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="76ce4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="76ce4-145">Request</span></span>
<span data-ttu-id="76ce4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76ce4-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="76ce4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="76ce4-147">Response</span></span>
<span data-ttu-id="76ce4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76ce4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




