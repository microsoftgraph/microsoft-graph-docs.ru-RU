---
title: Действие updateSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55180fcad1ae6ec5064a1ca8202be7e9c3862ccb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945846"
---
# <a name="updatesettings-action"></a><span data-ttu-id="e37b5-103">Действие updateSettings</span><span class="sxs-lookup"><span data-stu-id="e37b5-103">updateSettings action</span></span>

> <span data-ttu-id="e37b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e37b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e37b5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e37b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e37b5-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e37b5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e37b5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e37b5-107">Prerequisites</span></span>
<span data-ttu-id="e37b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e37b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e37b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e37b5-110">Permission type</span></span>|<span data-ttu-id="e37b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e37b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e37b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e37b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e37b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e37b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e37b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e37b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e37b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e37b5-115">Not supported.</span></span>|
|<span data-ttu-id="e37b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e37b5-116">Application</span></span>|<span data-ttu-id="e37b5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e37b5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e37b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e37b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="e37b5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e37b5-119">Request headers</span></span>
|<span data-ttu-id="e37b5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e37b5-120">Header</span></span>|<span data-ttu-id="e37b5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e37b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e37b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e37b5-122">Authorization</span></span>|<span data-ttu-id="e37b5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e37b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e37b5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e37b5-124">Accept</span></span>|<span data-ttu-id="e37b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e37b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e37b5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e37b5-126">Request body</span></span>
<span data-ttu-id="e37b5-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e37b5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e37b5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e37b5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e37b5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e37b5-129">Property</span></span>|<span data-ttu-id="e37b5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e37b5-130">Type</span></span>|<span data-ttu-id="e37b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e37b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e37b5-132">параметры</span><span class="sxs-lookup"><span data-stu-id="e37b5-132">settings</span></span>|<span data-ttu-id="e37b5-133">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e37b5-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="e37b5-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e37b5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e37b5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e37b5-135">Response</span></span>
<span data-ttu-id="e37b5-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e37b5-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e37b5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e37b5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e37b5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e37b5-138">Request</span></span>
<span data-ttu-id="e37b5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e37b5-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/updateSettings

Content-type: application/json
Content-length: 252

{
  "settings": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e37b5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e37b5-140">Response</span></span>
<span data-ttu-id="e37b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e37b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





