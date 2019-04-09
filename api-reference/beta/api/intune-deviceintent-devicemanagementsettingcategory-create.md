---
title: Создание Девицеманажементсеттингкатегори
description: Создание нового объекта Девицеманажементсеттингкатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7e9ee98d431d102e381719957ef9baa6859a0eb
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524136"
---
# <a name="create-devicemanagementsettingcategory"></a><span data-ttu-id="b0eeb-103">Создание Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="b0eeb-103">Create deviceManagementSettingCategory</span></span>

> <span data-ttu-id="b0eeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0eeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0eeb-106">Создание нового объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="b0eeb-106">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0eeb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0eeb-107">Prerequisites</span></span>
<span data-ttu-id="b0eeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0eeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0eeb-110">Permission type</span></span>|<span data-ttu-id="b0eeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0eeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0eeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0eeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0eeb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0eeb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0eeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0eeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0eeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-115">Not supported.</span></span>|
|<span data-ttu-id="b0eeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0eeb-116">Application</span></span>|<span data-ttu-id="b0eeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0eeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0eeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="b0eeb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0eeb-119">Request headers</span></span>
|<span data-ttu-id="b0eeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0eeb-120">Header</span></span>|<span data-ttu-id="b0eeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0eeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0eeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0eeb-122">Authorization</span></span>|<span data-ttu-id="b0eeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0eeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0eeb-124">Accept</span></span>|<span data-ttu-id="b0eeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0eeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0eeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0eeb-126">Request body</span></span>
<span data-ttu-id="b0eeb-127">В тексте запроса добавьте представление объекта Девицеманажементсеттингкатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-127">In the request body, supply a JSON representation for the deviceManagementSettingCategory object.</span></span>

<span data-ttu-id="b0eeb-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингкатегори.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-128">The following table shows the properties that are required when you create the deviceManagementSettingCategory.</span></span>

|<span data-ttu-id="b0eeb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0eeb-129">Property</span></span>|<span data-ttu-id="b0eeb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b0eeb-130">Type</span></span>|<span data-ttu-id="b0eeb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b0eeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0eeb-132">id</span><span class="sxs-lookup"><span data-stu-id="b0eeb-132">id</span></span>|<span data-ttu-id="b0eeb-133">String</span><span class="sxs-lookup"><span data-stu-id="b0eeb-133">String</span></span>|<span data-ttu-id="b0eeb-134">Идентификатор категории</span><span class="sxs-lookup"><span data-stu-id="b0eeb-134">The category ID</span></span>|
|<span data-ttu-id="b0eeb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b0eeb-135">displayName</span></span>|<span data-ttu-id="b0eeb-136">String</span><span class="sxs-lookup"><span data-stu-id="b0eeb-136">String</span></span>|<span data-ttu-id="b0eeb-137">Имя категории</span><span class="sxs-lookup"><span data-stu-id="b0eeb-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="b0eeb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0eeb-138">Response</span></span>
<span data-ttu-id="b0eeb-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-139">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0eeb-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b0eeb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0eeb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0eeb-141">Request</span></span>
<span data-ttu-id="b0eeb-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/categories
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="b0eeb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0eeb-143">Response</span></span>
<span data-ttu-id="b0eeb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0eeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







