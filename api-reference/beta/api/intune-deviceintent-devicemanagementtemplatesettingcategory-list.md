---
title: Список Девицеманажементтемплатесеттингкатегориес
description: Список свойств и связей объектов Девицеманажементтемплатесеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50d3a0f1a865b1028bb1e7daf26dd4af3ae7e65f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188936"
---
# <a name="list-devicemanagementtemplatesettingcategories"></a><span data-ttu-id="c39cb-103">Список Девицеманажементтемплатесеттингкатегориес</span><span class="sxs-lookup"><span data-stu-id="c39cb-103">List deviceManagementTemplateSettingCategories</span></span>

> <span data-ttu-id="c39cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c39cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c39cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c39cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c39cb-106">Список свойств и связей объектов [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c39cb-106">List properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c39cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c39cb-107">Prerequisites</span></span>
<span data-ttu-id="c39cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c39cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c39cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c39cb-110">Permission type</span></span>|<span data-ttu-id="c39cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c39cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c39cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c39cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c39cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c39cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c39cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c39cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c39cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c39cb-115">Not supported.</span></span>|
|<span data-ttu-id="c39cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c39cb-116">Application</span></span>|<span data-ttu-id="c39cb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c39cb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c39cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c39cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="c39cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c39cb-119">Request headers</span></span>
|<span data-ttu-id="c39cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c39cb-120">Header</span></span>|<span data-ttu-id="c39cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c39cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c39cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c39cb-122">Authorization</span></span>|<span data-ttu-id="c39cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c39cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c39cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c39cb-124">Accept</span></span>|<span data-ttu-id="c39cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c39cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c39cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c39cb-126">Request body</span></span>
<span data-ttu-id="c39cb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c39cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c39cb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c39cb-128">Response</span></span>
<span data-ttu-id="c39cb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c39cb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c39cb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c39cb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c39cb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c39cb-131">Request</span></span>
<span data-ttu-id="c39cb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c39cb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
```

### <a name="response"></a><span data-ttu-id="c39cb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c39cb-133">Response</span></span>
<span data-ttu-id="c39cb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c39cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
      "id": "cd213562-3562-cd21-6235-21cd623521cd",
      "displayName": "Display Name value"
    }
  ]
}
```




