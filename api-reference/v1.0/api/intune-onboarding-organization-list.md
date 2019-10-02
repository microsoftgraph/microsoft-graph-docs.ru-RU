---
title: Список организаций
description: Список свойств и связей объектов organization.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9edd123dc9c71a6da742e4acaf76c2ad271187a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362157"
---
# <a name="list-organizations"></a><span data-ttu-id="36e85-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="36e85-103">List organizations</span></span>

> <span data-ttu-id="36e85-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36e85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36e85-105">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="36e85-105">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36e85-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36e85-106">Prerequisites</span></span>
<span data-ttu-id="36e85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e85-109">Permission type</span></span>|<span data-ttu-id="36e85-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e85-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36e85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36e85-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e85-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="36e85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e85-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36e85-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e85-114">Not supported.</span></span>|
|<span data-ttu-id="36e85-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36e85-115">Application</span></span>|<span data-ttu-id="36e85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e85-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36e85-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e85-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="36e85-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36e85-118">Request headers</span></span>
|<span data-ttu-id="36e85-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36e85-119">Header</span></span>|<span data-ttu-id="36e85-120">Значение</span><span class="sxs-lookup"><span data-stu-id="36e85-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36e85-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36e85-121">Authorization</span></span>|<span data-ttu-id="36e85-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e85-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36e85-123">Accept</span><span class="sxs-lookup"><span data-stu-id="36e85-123">Accept</span></span>|<span data-ttu-id="36e85-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36e85-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36e85-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36e85-125">Request body</span></span>
<span data-ttu-id="36e85-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36e85-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36e85-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="36e85-127">Response</span></span>
<span data-ttu-id="36e85-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36e85-128">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e85-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36e85-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="36e85-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e85-130">Request</span></span>
<span data-ttu-id="36e85-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e85-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="36e85-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e85-132">Response</span></span>
<span data-ttu-id="36e85-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36e85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




