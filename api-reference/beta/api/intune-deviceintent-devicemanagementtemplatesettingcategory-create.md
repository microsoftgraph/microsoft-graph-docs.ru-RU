---
title: Создание Девицеманажементтемплатесеттингкатегори
description: Создание нового объекта Девицеманажементтемплатесеттингкатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35bdbf02baad1c41ea88fb71df802b1056931553
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466590"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="fc156-103">Создание Девицеманажементтемплатесеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="fc156-103">Create deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="fc156-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc156-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc156-106">Создание нового объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="fc156-106">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc156-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc156-107">Prerequisites</span></span>
<span data-ttu-id="fc156-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc156-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc156-110">Permission type</span></span>|<span data-ttu-id="fc156-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc156-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc156-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc156-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc156-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc156-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc156-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc156-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc156-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc156-115">Not supported.</span></span>|
|<span data-ttu-id="fc156-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc156-116">Application</span></span>|<span data-ttu-id="fc156-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc156-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc156-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc156-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="fc156-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc156-119">Request headers</span></span>
|<span data-ttu-id="fc156-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc156-120">Header</span></span>|<span data-ttu-id="fc156-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc156-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc156-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc156-122">Authorization</span></span>|<span data-ttu-id="fc156-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc156-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc156-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc156-124">Accept</span></span>|<span data-ttu-id="fc156-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc156-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc156-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc156-126">Request body</span></span>
<span data-ttu-id="fc156-127">В тексте запроса добавьте представление объекта Девицеманажементтемплатесеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc156-127">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="fc156-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплатесеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="fc156-128">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="fc156-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc156-129">Property</span></span>|<span data-ttu-id="fc156-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc156-130">Type</span></span>|<span data-ttu-id="fc156-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc156-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc156-132">id</span><span class="sxs-lookup"><span data-stu-id="fc156-132">id</span></span>|<span data-ttu-id="fc156-133">String</span><span class="sxs-lookup"><span data-stu-id="fc156-133">String</span></span>|<span data-ttu-id="fc156-134">Идентификатор категории, наСледуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="fc156-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="fc156-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fc156-135">displayName</span></span>|<span data-ttu-id="fc156-136">String</span><span class="sxs-lookup"><span data-stu-id="fc156-136">String</span></span>|<span data-ttu-id="fc156-137">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="fc156-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fc156-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc156-138">Response</span></span>
<span data-ttu-id="fc156-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc156-139">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc156-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fc156-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc156-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc156-141">Request</span></span>
<span data-ttu-id="fc156-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc156-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="fc156-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc156-143">Response</span></span>
<span data-ttu-id="fc156-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc156-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 170

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value"
}
```





