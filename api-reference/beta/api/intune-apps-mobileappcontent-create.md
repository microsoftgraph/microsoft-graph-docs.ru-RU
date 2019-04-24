---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba9b744b85644e554993801c801da5d0c23b3409
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489606"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="3be03-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3be03-103">Create mobileAppContent</span></span>

> <span data-ttu-id="3be03-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3be03-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3be03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3be03-106">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3be03-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3be03-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3be03-107">Prerequisites</span></span>
<span data-ttu-id="3be03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be03-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3be03-110">Permission type</span></span>|<span data-ttu-id="3be03-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3be03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3be03-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3be03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3be03-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be03-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3be03-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3be03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3be03-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be03-115">Not supported.</span></span>|
|<span data-ttu-id="3be03-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3be03-116">Application</span></span>|<span data-ttu-id="3be03-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3be03-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3be03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="3be03-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3be03-119">Request headers</span></span>
|<span data-ttu-id="3be03-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3be03-120">Header</span></span>|<span data-ttu-id="3be03-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3be03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3be03-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3be03-122">Authorization</span></span>|<span data-ttu-id="3be03-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3be03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3be03-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3be03-124">Accept</span></span>|<span data-ttu-id="3be03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3be03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3be03-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3be03-126">Request body</span></span>
<span data-ttu-id="3be03-127">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3be03-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="3be03-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="3be03-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="3be03-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3be03-129">Property</span></span>|<span data-ttu-id="3be03-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3be03-130">Type</span></span>|<span data-ttu-id="3be03-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3be03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be03-132">id</span><span class="sxs-lookup"><span data-stu-id="3be03-132">id</span></span>|<span data-ttu-id="3be03-133">String</span><span class="sxs-lookup"><span data-stu-id="3be03-133">String</span></span>|<span data-ttu-id="3be03-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="3be03-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="3be03-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be03-135">Response</span></span>
<span data-ttu-id="3be03-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3be03-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be03-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3be03-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3be03-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3be03-138">Request</span></span>
<span data-ttu-id="3be03-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3be03-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="3be03-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be03-140">Response</span></span>
<span data-ttu-id="3be03-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3be03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





