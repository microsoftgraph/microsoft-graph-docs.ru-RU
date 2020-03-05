---
title: действие Упдатедефинитионвалуес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c1ec5462365f6c28ff7f72bc47f0bb31f684fb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465193"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="2b6d6-103">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="2b6d6-103">updateDefinitionValues action</span></span>

<span data-ttu-id="2b6d6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b6d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b6d6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b6d6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6d6-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6d6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b6d6-108">Prerequisites</span></span>
<span data-ttu-id="2b6d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b6d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6d6-111">Permission type</span></span>|<span data-ttu-id="2b6d6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b6d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6d6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b6d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6d6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6d6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2b6d6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b6d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-116">Not supported.</span></span>|
|<span data-ttu-id="2b6d6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b6d6-117">Application</span></span>|<span data-ttu-id="2b6d6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6d6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b6d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="2b6d6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b6d6-120">Request headers</span></span>
|<span data-ttu-id="2b6d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b6d6-121">Header</span></span>|<span data-ttu-id="2b6d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b6d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6d6-123">Authorization</span></span>|<span data-ttu-id="2b6d6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b6d6-125">Accept</span></span>|<span data-ttu-id="2b6d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b6d6-127">Request body</span></span>
<span data-ttu-id="2b6d6-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2b6d6-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2b6d6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b6d6-130">Property</span></span>|<span data-ttu-id="2b6d6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b6d6-131">Type</span></span>|<span data-ttu-id="2b6d6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6d6-133">Добавлено</span><span class="sxs-lookup"><span data-stu-id="2b6d6-133">added</span></span>|<span data-ttu-id="2b6d6-134">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2b6d6-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="2b6d6-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-135">Not yet documented</span></span>|
|<span data-ttu-id="2b6d6-136">обновленный</span><span class="sxs-lookup"><span data-stu-id="2b6d6-136">updated</span></span>|<span data-ttu-id="2b6d6-137">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2b6d6-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="2b6d6-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-138">Not yet documented</span></span>|
|<span data-ttu-id="2b6d6-139">делетедидс</span><span class="sxs-lookup"><span data-stu-id="2b6d6-139">deletedIds</span></span>|<span data-ttu-id="2b6d6-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2b6d6-140">String collection</span></span>|<span data-ttu-id="2b6d6-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b6d6-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2b6d6-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b6d6-142">Response</span></span>
<span data-ttu-id="2b6d6-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2b6d6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="2b6d6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b6d6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b6d6-145">Request</span></span>
<span data-ttu-id="2b6d6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b6d6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b6d6-147">Response</span></span>
<span data-ttu-id="2b6d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b6d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





