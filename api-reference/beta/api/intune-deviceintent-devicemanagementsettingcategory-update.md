---
title: Обновление Девицеманажементсеттингкатегори
description: Обновление свойств объекта Девицеманажементсеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 438489de88b1e712c7f6e937f096aba9755c639b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959959"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="5fc06-103">Обновление Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="5fc06-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="5fc06-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fc06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fc06-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fc06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fc06-106">Обновление свойств объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="5fc06-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fc06-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5fc06-107">Prerequisites</span></span>
<span data-ttu-id="5fc06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fc06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fc06-110">Permission type</span></span>|<span data-ttu-id="5fc06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fc06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fc06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fc06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fc06-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc06-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fc06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fc06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fc06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fc06-115">Not supported.</span></span>|
|<span data-ttu-id="5fc06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fc06-116">Application</span></span>|<span data-ttu-id="5fc06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fc06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fc06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fc06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5fc06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fc06-119">Request headers</span></span>
|<span data-ttu-id="5fc06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5fc06-120">Header</span></span>|<span data-ttu-id="5fc06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5fc06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fc06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fc06-122">Authorization</span></span>|<span data-ttu-id="5fc06-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fc06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fc06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5fc06-124">Accept</span></span>|<span data-ttu-id="5fc06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fc06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fc06-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5fc06-126">Request body</span></span>
<span data-ttu-id="5fc06-127">В тексте запроса добавьте представление объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fc06-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="5fc06-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="5fc06-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="5fc06-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fc06-129">Property</span></span>|<span data-ttu-id="5fc06-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5fc06-130">Type</span></span>|<span data-ttu-id="5fc06-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fc06-132">id</span><span class="sxs-lookup"><span data-stu-id="5fc06-132">id</span></span>|<span data-ttu-id="5fc06-133">String</span><span class="sxs-lookup"><span data-stu-id="5fc06-133">String</span></span>|<span data-ttu-id="5fc06-134">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="5fc06-134">The category ID</span></span>|
|<span data-ttu-id="5fc06-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5fc06-135">displayName</span></span>|<span data-ttu-id="5fc06-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5fc06-136">String</span></span>|<span data-ttu-id="5fc06-137">Имя категории</span><span class="sxs-lookup"><span data-stu-id="5fc06-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="5fc06-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fc06-138">Response</span></span>
<span data-ttu-id="5fc06-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5fc06-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc06-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5fc06-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fc06-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fc06-141">Request</span></span>
<span data-ttu-id="5fc06-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fc06-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="5fc06-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fc06-143">Response</span></span>
<span data-ttu-id="5fc06-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5fc06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value"
}
```





