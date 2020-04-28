---
title: Список Девицеманажементсеттингкатегориес
description: Список свойств и связей объектов Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a36b6554d5a56b4819e1dbfaf258f42059b62065
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427856"
---
# <a name="list-devicemanagementsettingcategories"></a><span data-ttu-id="3ed25-103">Список Девицеманажементсеттингкатегориес</span><span class="sxs-lookup"><span data-stu-id="3ed25-103">List deviceManagementSettingCategories</span></span>

<span data-ttu-id="3ed25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ed25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ed25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ed25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed25-107">Список свойств и связей объектов [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3ed25-107">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ed25-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ed25-108">Prerequisites</span></span>
<span data-ttu-id="3ed25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ed25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ed25-111">Permission type</span></span>|<span data-ttu-id="3ed25-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ed25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ed25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ed25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ed25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ed25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ed25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ed25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed25-116">Not supported.</span></span>|
|<span data-ttu-id="3ed25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ed25-117">Application</span></span>|<span data-ttu-id="3ed25-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed25-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ed25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ed25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="3ed25-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ed25-120">Request headers</span></span>
|<span data-ttu-id="3ed25-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ed25-121">Header</span></span>|<span data-ttu-id="3ed25-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ed25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ed25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ed25-123">Authorization</span></span>|<span data-ttu-id="3ed25-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ed25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ed25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ed25-125">Accept</span></span>|<span data-ttu-id="3ed25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ed25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ed25-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ed25-127">Request body</span></span>
<span data-ttu-id="3ed25-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ed25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed25-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ed25-129">Response</span></span>
<span data-ttu-id="3ed25-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ed25-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ed25-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3ed25-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ed25-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ed25-132">Request</span></span>
<span data-ttu-id="3ed25-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ed25-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/categories
```

### <a name="response"></a><span data-ttu-id="3ed25-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ed25-134">Response</span></span>
<span data-ttu-id="3ed25-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ed25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
      "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
      "displayName": "Display Name value",
      "hasRequiredSetting": true
    }
  ]
}
```



