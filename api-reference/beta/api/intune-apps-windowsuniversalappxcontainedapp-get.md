---
title: Получение Виндовсуниверсалаппксконтаинедапп
description: Чтение свойств и связей объекта Виндовсуниверсалаппксконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bed5522578cee4f414e352b73fcb295e106e1ec5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976633"
---
# <a name="get-windowsuniversalappxcontainedapp"></a><span data-ttu-id="fa354-103">Получение Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="fa354-103">Get windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="fa354-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa354-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa354-106">Чтение свойств и связей объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fa354-106">Read properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa354-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa354-107">Prerequisites</span></span>
<span data-ttu-id="fa354-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa354-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa354-110">Permission type</span></span>|<span data-ttu-id="fa354-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa354-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa354-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa354-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa354-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa354-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa354-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa354-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa354-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa354-115">Not supported.</span></span>|
|<span data-ttu-id="fa354-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa354-116">Application</span></span>|<span data-ttu-id="fa354-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa354-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa354-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa354-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa354-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa354-119">Optional query parameters</span></span>
<span data-ttu-id="fa354-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa354-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa354-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa354-121">Request headers</span></span>
|<span data-ttu-id="fa354-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa354-122">Header</span></span>|<span data-ttu-id="fa354-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fa354-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa354-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa354-124">Authorization</span></span>|<span data-ttu-id="fa354-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa354-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa354-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fa354-126">Accept</span></span>|<span data-ttu-id="fa354-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa354-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa354-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa354-128">Request body</span></span>
<span data-ttu-id="fa354-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa354-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa354-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa354-130">Response</span></span>
<span data-ttu-id="fa354-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa354-131">If successful, this method returns a `200 OK` response code and [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa354-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fa354-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa354-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa354-133">Request</span></span>
<span data-ttu-id="fa354-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa354-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="fa354-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa354-135">Response</span></span>
<span data-ttu-id="fa354-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa354-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
    "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
    "appUserModelId": "App User Model Id value"
  }
}
```




