---
title: действие Упдатедефинитионвалуес
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57ca380359c1323cc0b3238f6f66b56e143afbd0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804480"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="8c025-103">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="8c025-103">updateDefinitionValues action</span></span>

> <span data-ttu-id="8c025-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c025-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c025-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c025-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c025-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c025-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c025-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c025-107">Prerequisites</span></span>
<span data-ttu-id="8c025-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c025-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c025-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c025-110">Permission type</span></span>|<span data-ttu-id="8c025-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c025-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c025-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c025-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c025-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c025-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8c025-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c025-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c025-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c025-115">Not supported.</span></span>|
|<span data-ttu-id="8c025-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c025-116">Application</span></span>|<span data-ttu-id="8c025-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c025-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c025-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c025-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="8c025-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c025-119">Request headers</span></span>
|<span data-ttu-id="8c025-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c025-120">Header</span></span>|<span data-ttu-id="8c025-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8c025-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c025-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c025-122">Authorization</span></span>|<span data-ttu-id="8c025-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c025-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c025-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8c025-124">Accept</span></span>|<span data-ttu-id="8c025-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c025-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c025-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c025-126">Request body</span></span>
<span data-ttu-id="8c025-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c025-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8c025-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8c025-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8c025-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c025-129">Property</span></span>|<span data-ttu-id="8c025-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8c025-130">Type</span></span>|<span data-ttu-id="8c025-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8c025-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c025-132">Добавлено</span><span class="sxs-lookup"><span data-stu-id="8c025-132">added</span></span>|<span data-ttu-id="8c025-133">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8c025-133">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="8c025-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c025-134">Not yet documented</span></span>|
|<span data-ttu-id="8c025-135">обновленный</span><span class="sxs-lookup"><span data-stu-id="8c025-135">updated</span></span>|<span data-ttu-id="8c025-136">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8c025-136">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="8c025-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c025-137">Not yet documented</span></span>|
|<span data-ttu-id="8c025-138">делетедидс</span><span class="sxs-lookup"><span data-stu-id="8c025-138">deletedIds</span></span>|<span data-ttu-id="8c025-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8c025-139">String collection</span></span>|<span data-ttu-id="8c025-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8c025-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c025-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c025-141">Response</span></span>
<span data-ttu-id="8c025-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c025-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c025-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8c025-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c025-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c025-144">Request</span></span>
<span data-ttu-id="8c025-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c025-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues

Content-type: application/json
Content-length: 759

{
  "added": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "updated": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "deletedIds": [
    "Deleted Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8c025-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c025-146">Response</span></span>
<span data-ttu-id="8c025-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c025-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




