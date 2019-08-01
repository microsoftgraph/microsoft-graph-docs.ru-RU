---
title: Список организаций
description: Список свойств и связей объектов organization.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 045dcb8635bcee2b71d40a8a1c3fe056f59eadfc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024058"
---
# <a name="list-organizations"></a><span data-ttu-id="24e5c-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="24e5c-103">List organizations</span></span>

> <span data-ttu-id="24e5c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24e5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24e5c-105">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="24e5c-105">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24e5c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24e5c-106">Prerequisites</span></span>
<span data-ttu-id="24e5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e5c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24e5c-109">Permission type</span></span>|<span data-ttu-id="24e5c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24e5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24e5c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24e5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24e5c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24e5c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="24e5c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24e5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24e5c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e5c-114">Not supported.</span></span>|
|<span data-ttu-id="24e5c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24e5c-115">Application</span></span>|<span data-ttu-id="24e5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24e5c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24e5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="24e5c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24e5c-118">Request headers</span></span>
|<span data-ttu-id="24e5c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24e5c-119">Header</span></span>|<span data-ttu-id="24e5c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="24e5c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24e5c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24e5c-121">Authorization</span></span>|<span data-ttu-id="24e5c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e5c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24e5c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="24e5c-123">Accept</span></span>|<span data-ttu-id="24e5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24e5c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24e5c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24e5c-125">Request body</span></span>
<span data-ttu-id="24e5c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24e5c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e5c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="24e5c-127">Response</span></span>
<span data-ttu-id="24e5c-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24e5c-128">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24e5c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="24e5c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="24e5c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="24e5c-130">Request</span></span>
<span data-ttu-id="24e5c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24e5c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="24e5c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e5c-132">Response</span></span>
<span data-ttu-id="24e5c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24e5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```



