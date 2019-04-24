---
title: Создание Девицеманажементинтентсеттингкатегори
description: Создание нового объекта Девицеманажементинтентсеттингкатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: add0d92a29f2bf2d29176e0d22dc68f7deb19a18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507835"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="ee195-103">Создание Девицеманажементинтентсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="ee195-103">Create deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="ee195-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee195-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee195-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee195-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee195-106">Создание нового объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="ee195-106">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee195-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee195-107">Prerequisites</span></span>
<span data-ttu-id="ee195-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee195-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee195-110">Permission type</span></span>|<span data-ttu-id="ee195-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee195-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee195-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee195-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee195-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee195-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee195-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee195-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee195-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee195-115">Not supported.</span></span>|
|<span data-ttu-id="ee195-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee195-116">Application</span></span>|<span data-ttu-id="ee195-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee195-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee195-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee195-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="ee195-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee195-119">Request headers</span></span>
|<span data-ttu-id="ee195-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee195-120">Header</span></span>|<span data-ttu-id="ee195-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee195-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee195-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee195-122">Authorization</span></span>|<span data-ttu-id="ee195-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee195-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee195-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee195-124">Accept</span></span>|<span data-ttu-id="ee195-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee195-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee195-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee195-126">Request body</span></span>
<span data-ttu-id="ee195-127">В тексте запроса добавьте представление объекта Девицеманажементинтентсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee195-127">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="ee195-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="ee195-128">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="ee195-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee195-129">Property</span></span>|<span data-ttu-id="ee195-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee195-130">Type</span></span>|<span data-ttu-id="ee195-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee195-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee195-132">id</span><span class="sxs-lookup"><span data-stu-id="ee195-132">id</span></span>|<span data-ttu-id="ee195-133">String</span><span class="sxs-lookup"><span data-stu-id="ee195-133">String</span></span>|<span data-ttu-id="ee195-134">Идентификатор категории, наСледуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ee195-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="ee195-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ee195-135">displayName</span></span>|<span data-ttu-id="ee195-136">String</span><span class="sxs-lookup"><span data-stu-id="ee195-136">String</span></span>|<span data-ttu-id="ee195-137">Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ee195-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ee195-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee195-138">Response</span></span>
<span data-ttu-id="ee195-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee195-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee195-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ee195-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee195-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee195-141">Request</span></span>
<span data-ttu-id="ee195-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee195-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ee195-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee195-143">Response</span></span>
<span data-ttu-id="ee195-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee195-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value"
}
```





