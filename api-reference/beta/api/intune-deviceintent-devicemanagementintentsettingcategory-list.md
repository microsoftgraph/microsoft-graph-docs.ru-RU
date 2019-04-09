---
title: Список Девицеманажементинтентсеттингкатегориес
description: Список свойств и связей объектов Девицеманажементинтентсеттингкатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19e568468da3a52f727f6d09c7639b1f17f36e52
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522316"
---
# <a name="list-devicemanagementintentsettingcategories"></a><span data-ttu-id="48cda-103">Список Девицеманажементинтентсеттингкатегориес</span><span class="sxs-lookup"><span data-stu-id="48cda-103">List deviceManagementIntentSettingCategories</span></span>

> <span data-ttu-id="48cda-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48cda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48cda-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48cda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48cda-106">Список свойств и связей объектов [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="48cda-106">List properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48cda-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48cda-107">Prerequisites</span></span>
<span data-ttu-id="48cda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48cda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48cda-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48cda-110">Permission type</span></span>|<span data-ttu-id="48cda-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48cda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48cda-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48cda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48cda-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="48cda-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="48cda-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48cda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48cda-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48cda-115">Not supported.</span></span>|
|<span data-ttu-id="48cda-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48cda-116">Application</span></span>|<span data-ttu-id="48cda-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48cda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48cda-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48cda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="48cda-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48cda-119">Request headers</span></span>
|<span data-ttu-id="48cda-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48cda-120">Header</span></span>|<span data-ttu-id="48cda-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48cda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48cda-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48cda-122">Authorization</span></span>|<span data-ttu-id="48cda-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48cda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48cda-124">Accept</span><span class="sxs-lookup"><span data-stu-id="48cda-124">Accept</span></span>|<span data-ttu-id="48cda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48cda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48cda-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48cda-126">Request body</span></span>
<span data-ttu-id="48cda-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48cda-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48cda-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="48cda-128">Response</span></span>
<span data-ttu-id="48cda-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48cda-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48cda-130">Пример</span><span class="sxs-lookup"><span data-stu-id="48cda-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="48cda-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="48cda-131">Request</span></span>
<span data-ttu-id="48cda-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48cda-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
```

### <a name="response"></a><span data-ttu-id="48cda-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="48cda-133">Response</span></span>
<span data-ttu-id="48cda-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48cda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
      "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
      "displayName": "Display Name value"
    }
  ]
}
```







