---
title: Создание Макманажедапппротектион
description: Создание нового объекта Макманажедапппротектион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb021c1d68acb30554d879b8f77e5bbf77c46ff8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192704"
---
# <a name="create-macmanagedappprotection"></a><span data-ttu-id="711ba-103">Создание Макманажедапппротектион</span><span class="sxs-lookup"><span data-stu-id="711ba-103">Create macManagedAppProtection</span></span>

> <span data-ttu-id="711ba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="711ba-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="711ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="711ba-106">Создание нового объекта [макманажедапппротектион](../resources/intune-policyset-macmanagedappprotection.md) .</span><span class="sxs-lookup"><span data-stu-id="711ba-106">Create a new [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="711ba-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="711ba-107">Prerequisites</span></span>
<span data-ttu-id="711ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="711ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="711ba-110">Permission type</span></span>|<span data-ttu-id="711ba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="711ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="711ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="711ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="711ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="711ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711ba-115">Not supported.</span></span>|
|<span data-ttu-id="711ba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="711ba-116">Application</span></span>|<span data-ttu-id="711ba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711ba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="711ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="711ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/macManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="711ba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="711ba-119">Request headers</span></span>
|<span data-ttu-id="711ba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="711ba-120">Header</span></span>|<span data-ttu-id="711ba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="711ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="711ba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="711ba-122">Authorization</span></span>|<span data-ttu-id="711ba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="711ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="711ba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="711ba-124">Accept</span></span>|<span data-ttu-id="711ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="711ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="711ba-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="711ba-126">Request body</span></span>
<span data-ttu-id="711ba-127">В тексте запроса добавьте представление объекта Макманажедапппротектион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="711ba-127">In the request body, supply a JSON representation for the macManagedAppProtection object.</span></span>

<span data-ttu-id="711ba-128">В следующей таблице приведены свойства, необходимые при создании Макманажедапппротектион.</span><span class="sxs-lookup"><span data-stu-id="711ba-128">The following table shows the properties that are required when you create the macManagedAppProtection.</span></span>

|<span data-ttu-id="711ba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="711ba-129">Property</span></span>|<span data-ttu-id="711ba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="711ba-130">Type</span></span>|<span data-ttu-id="711ba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="711ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="711ba-132">id</span><span class="sxs-lookup"><span data-stu-id="711ba-132">id</span></span>|<span data-ttu-id="711ba-133">String</span><span class="sxs-lookup"><span data-stu-id="711ba-133">String</span></span>|<span data-ttu-id="711ba-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="711ba-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="711ba-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="711ba-135">Response</span></span>
<span data-ttu-id="711ba-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макманажедапппротектион](../resources/intune-policyset-macmanagedappprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="711ba-136">If successful, this method returns a `201 Created` response code and a [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="711ba-137">Пример</span><span class="sxs-lookup"><span data-stu-id="711ba-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="711ba-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="711ba-138">Request</span></span>
<span data-ttu-id="711ba-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="711ba-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/macManagedAppProtections
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection"
}
```

### <a name="response"></a><span data-ttu-id="711ba-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="711ba-140">Response</span></span>
<span data-ttu-id="711ba-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="711ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection",
  "id": "bb139531-9531-bb13-3195-13bb319513bb"
}
```




