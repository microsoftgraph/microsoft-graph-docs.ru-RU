---
title: Создание Девицеманажементсеттингкатегори
description: Создание нового объекта Девицеманажементсеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26b33ef95c628674d66d27f3b610670d2cc37507
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162318"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="18f00-103">Создание Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="18f00-103">Create deviceManagementSettingCategory</span></span>

> <span data-ttu-id="18f00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18f00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18f00-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18f00-106">Создание нового объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="18f00-106">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18f00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18f00-107">Prerequisites</span></span>
<span data-ttu-id="18f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18f00-110">Permission type</span></span>|<span data-ttu-id="18f00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18f00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18f00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18f00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18f00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18f00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18f00-115">Not supported.</span></span>|
|<span data-ttu-id="18f00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18f00-116">Application</span></span>|<span data-ttu-id="18f00-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f00-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18f00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="18f00-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18f00-119">Request headers</span></span>
|<span data-ttu-id="18f00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18f00-120">Header</span></span>|<span data-ttu-id="18f00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18f00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f00-122">Authorization</span></span>|<span data-ttu-id="18f00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18f00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18f00-124">Accept</span></span>|<span data-ttu-id="18f00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18f00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f00-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18f00-126">Request body</span></span>
<span data-ttu-id="18f00-127">В тексте запроса добавьте представление объекта Девицеманажементсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18f00-127">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="18f00-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="18f00-128">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="18f00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18f00-129">Property</span></span>|<span data-ttu-id="18f00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18f00-130">Type</span></span>|<span data-ttu-id="18f00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18f00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f00-132">id</span><span class="sxs-lookup"><span data-stu-id="18f00-132">id</span></span>|<span data-ttu-id="18f00-133">String</span><span class="sxs-lookup"><span data-stu-id="18f00-133">String</span></span>|<span data-ttu-id="18f00-134">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="18f00-134">The category ID</span></span>|
|<span data-ttu-id="18f00-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18f00-135">displayName</span></span>|<span data-ttu-id="18f00-136">Строка</span><span class="sxs-lookup"><span data-stu-id="18f00-136">String</span></span>|<span data-ttu-id="18f00-137">Имя категории</span><span class="sxs-lookup"><span data-stu-id="18f00-137">The category name</span></span>|
|<span data-ttu-id="18f00-138">хасрекуиредсеттинг</span><span class="sxs-lookup"><span data-stu-id="18f00-138">hasRequiredSetting</span></span>|<span data-ttu-id="18f00-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="18f00-139">Boolean</span></span>|<span data-ttu-id="18f00-140">Категория содержит параметры, необходимые для верхнего уровня</span><span class="sxs-lookup"><span data-stu-id="18f00-140">The category contains top level required setting</span></span>|



## <a name="response"></a><span data-ttu-id="18f00-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="18f00-141">Response</span></span>
<span data-ttu-id="18f00-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18f00-142">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f00-143">Пример</span><span class="sxs-lookup"><span data-stu-id="18f00-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="18f00-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="18f00-144">Request</span></span>
<span data-ttu-id="18f00-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18f00-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18f00-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="18f00-146">Response</span></span>
<span data-ttu-id="18f00-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18f00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





