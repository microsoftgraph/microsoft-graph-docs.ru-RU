---
title: Получение Девицеманажементтемплатесеттингкатегори
description: Чтение свойств и связей объекта Девицеманажементтемплатесеттингкатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b270af753d1ba9e67d0a75a02bd379705d48837
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945440"
---
# <a name="get-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="80bee-103">Получение Девицеманажементтемплатесеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="80bee-103">Get deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="80bee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80bee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80bee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80bee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80bee-106">Чтение свойств и связей объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="80bee-106">Read properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80bee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="80bee-107">Prerequisites</span></span>
<span data-ttu-id="80bee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80bee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80bee-110">Permission type</span></span>|<span data-ttu-id="80bee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80bee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80bee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80bee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80bee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="80bee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80bee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80bee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80bee-115">Not supported.</span></span>|
|<span data-ttu-id="80bee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80bee-116">Application</span></span>|<span data-ttu-id="80bee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80bee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80bee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80bee-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80bee-119">Optional query parameters</span></span>
<span data-ttu-id="80bee-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="80bee-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80bee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80bee-121">Request headers</span></span>
|<span data-ttu-id="80bee-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80bee-122">Header</span></span>|<span data-ttu-id="80bee-123">Значение</span><span class="sxs-lookup"><span data-stu-id="80bee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80bee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80bee-124">Authorization</span></span>|<span data-ttu-id="80bee-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80bee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80bee-126">Accept</span><span class="sxs-lookup"><span data-stu-id="80bee-126">Accept</span></span>|<span data-ttu-id="80bee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80bee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80bee-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80bee-128">Request body</span></span>
<span data-ttu-id="80bee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80bee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80bee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="80bee-130">Response</span></span>
<span data-ttu-id="80bee-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80bee-131">If successful, this method returns a `200 OK` response code and [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80bee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="80bee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="80bee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="80bee-133">Request</span></span>
<span data-ttu-id="80bee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80bee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="80bee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="80bee-135">Response</span></span>
<span data-ttu-id="80bee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80bee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
    "id": "cd213562-3562-cd21-6235-21cd623521cd",
    "displayName": "Display Name value"
  }
}
```





