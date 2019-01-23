---
title: Get mobileAppContent
description: Чтение свойств и связей объекта mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9df3f77232a17a1ff1c10672e0c17b3e39ec64c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416904"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="8e93d-103">Get mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8e93d-103">Get mobileAppContent</span></span>

> <span data-ttu-id="8e93d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e93d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e93d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e93d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e93d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e93d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e93d-107">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8e93d-107">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e93d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8e93d-108">Prerequisites</span></span>
<span data-ttu-id="8e93d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e93d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e93d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e93d-111">Permission type</span></span>|<span data-ttu-id="8e93d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e93d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e93d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e93d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e93d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e93d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8e93d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e93d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e93d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e93d-116">Not supported.</span></span>|
|<span data-ttu-id="8e93d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e93d-117">Application</span></span>|<span data-ttu-id="8e93d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e93d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e93d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e93d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e93d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e93d-120">Optional query parameters</span></span>
<span data-ttu-id="8e93d-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e93d-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e93d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e93d-122">Request headers</span></span>
|<span data-ttu-id="8e93d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e93d-123">Header</span></span>|<span data-ttu-id="8e93d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8e93d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e93d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e93d-125">Authorization</span></span>|<span data-ttu-id="8e93d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e93d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e93d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8e93d-127">Accept</span></span>|<span data-ttu-id="8e93d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8e93d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e93d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e93d-129">Request body</span></span>
<span data-ttu-id="8e93d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e93d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e93d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e93d-131">Response</span></span>
<span data-ttu-id="8e93d-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8e93d-132">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e93d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8e93d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e93d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e93d-134">Request</span></span>
<span data-ttu-id="8e93d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e93d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="8e93d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e93d-136">Response</span></span>
<span data-ttu-id="8e93d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8e93d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```




