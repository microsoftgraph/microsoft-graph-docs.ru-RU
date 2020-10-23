---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c043b065d37434d9f7072d610c39a63dfd05138
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695980"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="bbb56-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bbb56-103">Update mobileAppContent</span></span>

<span data-ttu-id="bbb56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbb56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbb56-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbb56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbb56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb56-107">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bbb56-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbb56-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bbb56-108">Prerequisites</span></span>
<span data-ttu-id="bbb56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbb56-111">Permission type</span></span>|<span data-ttu-id="bbb56-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbb56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbb56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbb56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbb56-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb56-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbb56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbb56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbb56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb56-116">Not supported.</span></span>|
|<span data-ttu-id="bbb56-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbb56-117">Application</span></span>|<span data-ttu-id="bbb56-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb56-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbb56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbb56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="bbb56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bbb56-120">Request headers</span></span>
|<span data-ttu-id="bbb56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbb56-121">Header</span></span>|<span data-ttu-id="bbb56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bbb56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbb56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbb56-123">Authorization</span></span>|<span data-ttu-id="bbb56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbb56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbb56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bbb56-125">Accept</span></span>|<span data-ttu-id="bbb56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbb56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbb56-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbb56-127">Request body</span></span>
<span data-ttu-id="bbb56-128">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbb56-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="bbb56-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bbb56-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="bbb56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbb56-130">Property</span></span>|<span data-ttu-id="bbb56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bbb56-131">Type</span></span>|<span data-ttu-id="bbb56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb56-133">id</span><span class="sxs-lookup"><span data-stu-id="bbb56-133">id</span></span>|<span data-ttu-id="bbb56-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bbb56-134">String</span></span>|<span data-ttu-id="bbb56-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="bbb56-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="bbb56-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb56-136">Response</span></span>
<span data-ttu-id="bbb56-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbb56-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb56-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bbb56-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbb56-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbb56-139">Request</span></span>
<span data-ttu-id="bbb56-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbb56-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="bbb56-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb56-141">Response</span></span>
<span data-ttu-id="bbb56-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbb56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





