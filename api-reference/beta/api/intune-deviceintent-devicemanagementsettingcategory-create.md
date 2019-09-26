---
title: Создание Девицеманажементсеттингкатегори
description: Создание нового объекта Девицеманажементсеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6265ffd4324cd761ad4d2076f9c677ce94df35dc
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185730"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="1b8e5-103">Создание Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="1b8e5-103">Create deviceManagementSettingCategory</span></span>

> <span data-ttu-id="1b8e5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b8e5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b8e5-106">Создание нового объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="1b8e5-106">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b8e5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b8e5-107">Prerequisites</span></span>
<span data-ttu-id="1b8e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b8e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b8e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b8e5-110">Permission type</span></span>|<span data-ttu-id="1b8e5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b8e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b8e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b8e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b8e5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8e5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b8e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b8e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b8e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-115">Not supported.</span></span>|
|<span data-ttu-id="1b8e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b8e5-116">Application</span></span>|<span data-ttu-id="1b8e5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8e5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b8e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b8e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="1b8e5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b8e5-119">Request headers</span></span>
|<span data-ttu-id="1b8e5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b8e5-120">Header</span></span>|<span data-ttu-id="1b8e5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b8e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b8e5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b8e5-122">Authorization</span></span>|<span data-ttu-id="1b8e5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b8e5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b8e5-124">Accept</span></span>|<span data-ttu-id="1b8e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b8e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b8e5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b8e5-126">Request body</span></span>
<span data-ttu-id="1b8e5-127">В тексте запроса добавьте представление объекта Девицеманажементсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-127">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="1b8e5-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-128">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="1b8e5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b8e5-129">Property</span></span>|<span data-ttu-id="1b8e5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b8e5-130">Type</span></span>|<span data-ttu-id="1b8e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b8e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8e5-132">id</span><span class="sxs-lookup"><span data-stu-id="1b8e5-132">id</span></span>|<span data-ttu-id="1b8e5-133">String</span><span class="sxs-lookup"><span data-stu-id="1b8e5-133">String</span></span>|<span data-ttu-id="1b8e5-134">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="1b8e5-134">The category ID</span></span>|
|<span data-ttu-id="1b8e5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1b8e5-135">displayName</span></span>|<span data-ttu-id="1b8e5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1b8e5-136">String</span></span>|<span data-ttu-id="1b8e5-137">Имя категории</span><span class="sxs-lookup"><span data-stu-id="1b8e5-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="1b8e5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b8e5-138">Response</span></span>
<span data-ttu-id="1b8e5-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-139">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b8e5-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1b8e5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b8e5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b8e5-141">Request</span></span>
<span data-ttu-id="1b8e5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="1b8e5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b8e5-143">Response</span></span>
<span data-ttu-id="1b8e5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b8e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value"
}
```




