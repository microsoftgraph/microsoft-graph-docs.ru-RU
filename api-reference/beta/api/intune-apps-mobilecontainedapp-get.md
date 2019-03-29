---
title: Получение Мобилеконтаинедапп
description: Чтение свойств и связей объекта Мобилеконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f991137debd56d64854362e79a8f3159c6a5eb9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964166"
---
# <a name="get-mobilecontainedapp"></a><span data-ttu-id="fce42-103">Получение Мобилеконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="fce42-103">Get mobileContainedApp</span></span>

> <span data-ttu-id="fce42-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fce42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fce42-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fce42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fce42-106">Чтение свойств и связей объекта [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fce42-106">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fce42-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fce42-107">Prerequisites</span></span>
<span data-ttu-id="fce42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fce42-110">Permission type</span></span>|<span data-ttu-id="fce42-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fce42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fce42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fce42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fce42-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fce42-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fce42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fce42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fce42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fce42-115">Not supported.</span></span>|
|<span data-ttu-id="fce42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fce42-116">Application</span></span>|<span data-ttu-id="fce42-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fce42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fce42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fce42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fce42-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fce42-119">Optional query parameters</span></span>
<span data-ttu-id="fce42-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fce42-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fce42-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fce42-121">Request headers</span></span>
|<span data-ttu-id="fce42-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fce42-122">Header</span></span>|<span data-ttu-id="fce42-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fce42-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fce42-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fce42-124">Authorization</span></span>|<span data-ttu-id="fce42-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fce42-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fce42-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fce42-126">Accept</span></span>|<span data-ttu-id="fce42-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fce42-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fce42-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fce42-128">Request body</span></span>
<span data-ttu-id="fce42-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fce42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fce42-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fce42-130">Response</span></span>
<span data-ttu-id="fce42-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fce42-131">If successful, this method returns a `200 OK` response code and [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce42-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fce42-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fce42-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fce42-133">Request</span></span>
<span data-ttu-id="fce42-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fce42-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="fce42-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fce42-135">Response</span></span>
<span data-ttu-id="fce42-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fce42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileContainedApp",
    "id": "3c02d875-d875-3c02-75d8-023c75d8023c"
  }
}
```




