---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed9a6facc72bc941b3e26a802d324e1354d339a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577023"
---
# <a name="list-devicecategories"></a><span data-ttu-id="17172-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="17172-103">List deviceCategories</span></span>

> <span data-ttu-id="17172-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17172-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17172-105">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="17172-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17172-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17172-106">Prerequisites</span></span>
<span data-ttu-id="17172-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17172-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17172-109">Permission type</span></span>|<span data-ttu-id="17172-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17172-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17172-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17172-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="17172-112">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="17172-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="17172-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="17172-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="17172-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17172-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17172-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17172-115">Not supported.</span></span>|
|<span data-ttu-id="17172-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17172-116">Application</span></span>|<span data-ttu-id="17172-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17172-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17172-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17172-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="17172-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17172-119">Request headers</span></span>
|<span data-ttu-id="17172-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17172-120">Header</span></span>|<span data-ttu-id="17172-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17172-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17172-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17172-122">Authorization</span></span>|<span data-ttu-id="17172-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17172-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17172-124">Accept</span><span class="sxs-lookup"><span data-stu-id="17172-124">Accept</span></span>|<span data-ttu-id="17172-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17172-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17172-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17172-126">Request body</span></span>
<span data-ttu-id="17172-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17172-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17172-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="17172-128">Response</span></span>
<span data-ttu-id="17172-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17172-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17172-130">Пример</span><span class="sxs-lookup"><span data-stu-id="17172-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="17172-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="17172-131">Request</span></span>
<span data-ttu-id="17172-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17172-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="17172-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="17172-133">Response</span></span>
<span data-ttu-id="17172-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17172-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



